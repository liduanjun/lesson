# gitlab 

用 gitlab 可以架设自己的 git 仓库。
我们这里使用 gitlab 架设 TeacherServer

## .gitlab-ci.yml

在项目中可以添加 .gitlab-ci.yml ， 这样就可以使用 持续集成 功能了。

每当项目推送到 gitlab 仓储的时候，gitlab 就会自动去执行 .gitlab-ci.yml
中的命令。这样可以实现 git 项目的自动编译，测试和部署。

安装 git 查看 [gitlab安装](服务器安装gitlab.md)

[.gitlab-ci.yml模板文件](.gitlab-ci.yml)