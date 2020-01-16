# 三种不同的验证码生成器

如图：

![](https://github.com/Benjeming/codeCheck/blob/master/images/chrome_qphCqKQqn4.png)

三种不同类型的验证码

1. 简单的字母

2. 简单的加减法

3. 常见的中文字符

   源码来自于 github 中的 https://github.com/lingd3/Captcha

将源码进行了简单的改写，改成了一个 checkServlet.java .

### 怎么调用?

> 1. <imag> 标签中的 src 属性 直接链接到 checkServlet.java

```jsp
 	    <img src="${pageContext.request.contextPath}/easyCheckServlet" title="图片验证码">
        <img src="${pageContext.request.contextPath}/checkCodeServlet" title="数字验证码">
        <img src="${pageContext.request.contextPath}/chineseCheckServlet" title="中文验证码">
```

