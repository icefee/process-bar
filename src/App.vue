<template>
  <div id="app">
    <div class="container">
      <div class="item">
        <div class="title">常规</div>
        <process-bar class="bar" :value="20"/>
        <process-bar class="bar" :value="40"/>
        <process-bar class="bar" :value="60"/>
        <process-bar class="bar" :value="80"/>
        <div class="source">
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">20</span><span class="code">"/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">40</span><span class="code">"/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">60</span><span class="code">"/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">80</span><span class="code">"/></span>
          </p>
        </div>
      </div>
      <div class="item">
        <div class="title">自定义前景色</div>
        <process-bar class="bar" :value="20" color="#ffab78"/>
        <process-bar class="bar" :value="50" color="green"/>
        <process-bar class="bar" :value="90" color="purple"/>
        <div class="source">
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">20</span><span class="code">"</span>&nbsp;<span class="attr">color</span><span class="code">="</span><span class="value">#ffab78</span><span class="code">"</span><span class="code">/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">50</span><span class="code">"</span>&nbsp;<span class="attr">color</span><span class="code">="</span><span class="value">green</span><span class="code">"</span><span class="code">/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">75</span><span class="code">"</span>&nbsp;<span class="attr">color</span><span class="code">="</span><span class="value">purple</span><span class="code">"</span><span class="code">/></span>
          </p>
        </div>
      </div>
      <div class="item">
        <div class="title">自定义背景色</div>
        <process-bar class="bar" :value="20" background="#000"/>
        <process-bar class="bar" :value="50" background="#efefef"/>
        <process-bar class="bar" :value="75" background="purple"/>
        <div class="source">
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">20</span><span class="code">"</span>&nbsp;<span class="attr">background</span><span class="code">="</span><span class="value">#000</span><span class="code">"</span><span class="code">/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">50</span><span class="code">"</span>&nbsp;<span class="attr">background</span><span class="code">="</span><span class="value">#222</span><span class="code">"</span><span class="code">/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">75</span><span class="code">"</span>&nbsp;<span class="attr">background</span><span class="code">="</span><span class="value">purple</span><span class="code">"</span><span class="code">/></span>
          </p>
        </div>
      </div>
      <div class="item">
        <div class="title">自定义高度</div>
        <process-bar class="bar" :value="30" :height="2"/>
        <process-bar class="bar" :value="60" :height="5"/>
        <process-bar class="bar" :value="90" :height="8"/>
        <div class="source">
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">30</span><span class="code">"</span>&nbsp;<span class="code">:</span><span class="attr">height</span><span class="code">="</span><span class="value">2</span><span class="code">"/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">60</span><span class="code">"</span>&nbsp;<span class="code">:</span><span class="attr">height</span><span class="code">="</span><span class="value">5</span><span class="code">"/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">90</span><span class="code">"</span>&nbsp;<span class="code">:</span><span class="attr">height</span><span class="code">="</span><span class="value">8</span><span class="code">"/></span>
          </p>
        </div>
      </div>
      <div class="item">
        <div class="title">带圆角</div>
        <process-bar class="bar" :value="40" :height="4" radius/>
        <process-bar class="bar" :value="40" color="purple" :height="8" radius/>
        <div class="source">
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">40</span><span class="code">"</span>&nbsp;<span class="code">:</span><span class="attr">height</span><span class="code">="</span><span class="value">4</span><span class="code">"</span>&nbsp;<span class="tag">radius</span><span class="code">/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">90</span><span class="code">"</span>&nbsp;<span class="code">:</span><span class="attr">height</span><span class="code">="</span><span class="value">8</span><span class="code">"</span>&nbsp;<span class="attr">color</span><span class="code">="</span><span class="value">purple</span><span class="code">"</span>&nbsp;<span class="tag">radius</span><span class="code">/></span>
          </p>
        </div>
      </div>
      <div class="item">
        <div class="title">带文本</div>
        <process-bar class="bar" :value="40" label/>
        <process-bar class="bar" :value="90" label/>
        <div class="source">
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">40</span><span class="code">"</span>&nbsp;<span class="tag">label</span><span class="code">/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">90</span><span class="code">"</span>&nbsp;<span class="tag">label</span><span class="code">/></span>
          </p>
        </div>
      </div>
      <div class="item">
        <div class="title">带高光特效</div>
        <process-bar class="bar" :value="40" highlight/>
        <process-bar class="bar" :value="60" color="#c78efa" :height="6" radius highlight/>
        <div class="source">
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">40</span><span class="code">"</span>&nbsp;<span class="tag">highlight</span><span class="code">/></span>
          </p>
          <p>
            <span class="code"><</span><span class="tag">process-bar</span>&nbsp;<span class="code">:</span><span class="attr">value</span><span class="code">="</span><span class="value">60</span><span class="code">"</span>&nbsp;<span class="code">:</span><span class="attr">color</span><span class="code">="</span><span class="value">#c78efa</span><span class="code">"</span>&nbsp;<span class="code">:</span><span class="attr">height</span><span class="code">="</span><span class="value">6</span><span class="code">"</span>&nbsp;<span class="tag">radius</span>&nbsp;<span class="tag">highlight</span><span class="code">/></span>
          </p>
        </div>
      </div>
      <div class="item">
        <div class="title">组件属性</div>
        <table>
          <colgroup>
            <col width="100">
            <col width="150">
            <col width="150">
          </colgroup>
          <thead>
            <tr>
              <th>属性</th>
              <th>类型</th>
              <th>默认值</th>
              <th>说明</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>value(必需)</td>
              <td>数字/Number</td>
              <td>0</td>
              <td>用来设置进度条的百分比</td>
            </tr>
            <tr>
              <td>label</td>
              <td>布尔/Boolean</td>
              <td>false</td>
              <td>是否显示进度文本</td>
            </tr>
            <tr>
              <td>color</td>
              <td>字符串/String</td>
              <td>#f78abc</td>
              <td>进度条的前景色, 可接受任何有效的颜色</td>
            </tr>
            <tr>
              <td>background</td>
              <td>字符串/String</td>
              <td>#ddd</td>
              <td>进度条的背景色, 可接受任何有效的颜色</td>
            </tr>
            <tr>
              <td>height</td>
              <td>数字/Number</td>
              <td>3</td>
              <td>进度条的高度</td>
            </tr>
            <tr>
              <td>radius</td>
              <td>布尔/Boolean</td>
              <td>false</td>
              <td>进度条边缘显示为圆角</td>
            </tr>
            <tr>
              <td>highlight</td>
              <td>布尔/Boolean</td>
              <td>false</td>
              <td>进度条显示动态高光</td>
            </tr>
          </tbody>
        </table>
        <div class="tips">
          <p>注意: 所有非字符串类型的属性都应该使用vuejs绑定属性的指令 v-bind 或者 : , 例如 <code>v-bind:value="50"</code> 或者 <code>:value="50"</code></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import processBar from './components/processbar'

export default {
  name: 'app',
  components: {
    processBar
  }
}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html, body {
  height: 100%;
}
#app {
  height: 100%;
  overflow-y: scroll;
  background: #eee;
}
.container {
  width: 750px;
  margin: 0 auto;
  padding: 30px;
  background: #fff;
  box-shadow: 2px 2px 20px 0 rgba(0, 0, 0, .12);
}
.item {
  margin-bottom: 40px;
}
.item .title {
  font-size: 14px;
  color: #777;
  margin-bottom: 20px;
}
.item .bar {
  margin-bottom: 30px;
}
.source {
  width: 100%;
  padding: 15px 20px;
  background: #222;
}
.source p {
  line-height: 30px;
}
.source span {
  font-size: 13px;
}
.source .code {
  color: #fff;
}
.source .tag {
  color: #e2777a;
}
.source .attr {
  color: #ea0e63;
}
.source .value {
  color: #1ab010;
}
.item table {
  width: 100%;
  border-spacing: 0;
  border-collapse: separate;
  font-size: 13px;
  text-align: center;
}
.item table th, .item table td {
  border: 1px solid #eee;
  padding: 10px 15px;
}
.tips {
  padding: 10px 0;
}
.tips p {
  font-size: 13px;
}
</style>
