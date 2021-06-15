# nuxt-vercel

nuxt 渲染模式为服务端渲染，可以使用vercel进行自动化部署。本项目为演示，步骤如下：

1.项目根目录创建vercel.json 内容为{
    "builds":[
        {
            "src":"nuxt.config.js",
            "use":"@nuxtjs/vercel-builder",
            "config":{}
        }
    ]
}

2.项目代码提交到github,忽略node_modules和.nuxt

3.进到vercel官网，地址为vercel.com，点overview,点导入，然后依次下一步，即可完成自动化部署。

ps：vercel本身是个服务器