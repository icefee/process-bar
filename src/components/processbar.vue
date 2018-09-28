<template>
	<div class="wrap">
		<div class="process" :style="barStyle">
			<div class="inner" :class="innerClasses" :style="innerStyle"></div>
		</div>
		<label v-if="label" :style="labelStyle">{{ value }}%</label>
	</div>
</template>

<script>
	export default {
		props: {
			value: {
				type: Number,
				required: true,
				default: 0
			},
			label: {
				type: Boolean,
				default: false
			},
			color: {
				type: String,
				default: '#f78abc'
			},
			background: {
				type: String,
				default: '#ddd'
			},
			height: {
				type: Number,
				default: 3
			},
			highlight: {
				type: Boolean,
				default: false
			},
			radius: {
				type: Boolean,
				default: false
			}
		},
		computed: {
			barStyle() {
				const styles = {
					backgroundColor: this.background,
					height: this.height + 'px'
				}

				if(this.radius) styles.borderRadius = this.height / 2 + 'px'

				return styles
			},
			innerClasses() {
				return {
					running: this.value < 100,
					highlight: this.highlight
				}
			},
			innerStyle() {
				const styles = {
					width: this.value + '%',
					background: this.color
				}

				if(this.radius) styles.borderRadius = this.height / 2 + 'px'

				return styles
			},
			labelStyle() {
				return {
					color: this.color
				}
			}
		}
	}
</script>

<style lang="less" scoped>
	.wrap {
		width: 100%;
		display: flex;
		align-items: center;
	}

	.process {
		width: 100%;
		overflow: hidden;

		.inner {
			position: relative;
			width: 0;
			height: 100%;
			transition: all .3s ease;
			overflow: hidden;
		}

		.highlight::after {
			content: '';
			position: absolute;
			width: 15px;
			height: 100%;
			box-shadow: 0 0 25px 15px #fff;
			top: 0;
			left: 0;
			background: #fff;
			opacity: .9;
			display: none;
		}

		.running::after {
			display: block;
			animation: process 5s infinite 0s ease;
		}
	}

	label {
		font-size: 14px;
	}

	@keyframes process {
		0% {
			left: -15px;
		}
		100% {
			left: calc(~'100% + 15px');
		}
	}
</style>