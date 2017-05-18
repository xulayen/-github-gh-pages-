# -github-gh-pages-
<div class="note">
        <div class="post">
            <div class="article">
                <h1 class="title">
                    在github上建立gh-pages分支</h1>
                <!-- 文章内容 -->
                <div class="show-content">
                    <h1>
                        在github上建立gh-pages分支</h1>
                    <pre class="hljs undefined"><code>为什么要建立gh-pages分支呢，因为github项目的静态页面解析需要这个名字的分支</code></pre>
                    <ul>
                        <li>进入到你想要上传的文件夹下：<br>
                            <code>cd text</code> </li>
                        <li>git初始化<br>
                            <code>git init</code> </li>
                        <li>创建gh-pages分支<br>
                            <code>git checkout --orphan gh-pages</code> </li>
                        <li>添加文件到暂存区<br>
                            <code>git add .</code> </li>
                        <li>
                            <p>
                                添加信息<br>
                                <code>git commit -m "This is add message"</code></p>
                            <blockquote>
                                <p>
                                    或者不写上面的<code>git add .</code>直接写 <code>git commit -a -m \"First pages commit\"</code>这个<code>-a</code>参数我查了之后说是对<code>git
                                        add .</code>的替代，但我不建议大家使用。</p>
                            </blockquote>
                        </li>
                        <li>
                            <p>
                                添加仓库<br>
                                <code>git remote add origin git@github.com:username/project.git</code></p>
                        </li>
                        <li>
                            <p>
                                部署你的项目到github<br>
                                <code>git push origin gh-pages</code></p>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
