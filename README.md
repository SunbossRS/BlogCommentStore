<center>
<h1> Talk! > </h1>
</center>
<center>
欢迎来到耀庄老弟的评论系统的储存器仓库。<br/>
现在是用的是依靠Vue.js框架的评论系统。<br/>
目前正处于开源空间GitHub。
</center>

---
### 状态标签
![issues](https://img.shields.io/github/issues/sunbossrs/suntalk_save.svg?style=flat-square)  
![use-type](https://img.shields.io/badge/use--type-vue.js-green.svg?style=flat-square)  
![stand-by](https://img.shields.io/badge/stand--by-vssue-green.svg?style=flat-square)  
![vue-type](https://img.shields.io/badge/vue--type-full-orange.svg?style=flat-square)  
![issue-output](https://img.shields.io/badge/issue--output-md5-lightgrey.svg?style=flat-square)

---
### 运作
> 网站和数据库运作正常。
<br/>

!> 发现错误: 
!> 发表评论时会发送两个。

---

#### 快速。
采用最先进的框架并使用Unpkg进行内容提供。

#### 好看。
凡事先靠颜值。评论系统使用的是非常养眼的绿色，很好看，Ui也设计的很好。

#### 运用省心。
当运用OAuth应用给这个仓库的Issues部进行添加Issue标题时，运用md5进行缩减或增长而不超50个字符。

#### 稳定。
使用Vue.js框架的完整版而不是用运行版。完整版版相对功能比运行版多一点。

#### 安全。
你们在允许OAuth应用时所看到的允许OAuth对你们做出任何作用，是对于黑客有可乘之机的。而这里的OAuth可是几乎不外泄，黑客无可乘之机。

#### 放心。
使用GitHub的域名，是附带了Https加密传输的协议，让你们用的放心。

---

<div id="vssue"></div>
<link rel="stylesheet" href="https://unpkg.com/vssue/dist/vssue.min.css">
<script src="https://unpkg.com/vue/dist/vue.min.js"></script>
<script src="https://unpkg.com/vssue/dist/vssue.github.min.js"></script>
<script src="https://cdn.bootcss.com/blueimp-md5/2.10.0/js/md5.min.js"></script>
  <script>
    var talk = SunTalk
    new Vue({
      el: '#vssue',
      render: h => h('Vssue', {
        props: {
          title: 'SunTalk',
          options: {
            owner: 'SunbossRS',
            repo: 'SunTalk_Save',
            clientId: '800a929ad18c8e90fdbc',
            clientSecret: '3dcb1cc3680b9b85ad4291367b4aafefd6806e58',
          },
        }
      })
    })
  </script>
