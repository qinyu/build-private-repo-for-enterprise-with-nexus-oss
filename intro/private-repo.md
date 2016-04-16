# 私服

仓库私服就是部署在企业内部的仓库服务，用于存储企业自己的交付件；并且通过代理间接访问到其他互联网上的仓库。这样就可以解决上述这些问题。

主流的私服有Nexus，Archiva，Artifactory等。关于它们之间的特性对比，请参考[Binary Repository Manager Feature Matrix
](https://binary-repositories-comparison.github.io/)。

私服最早主要用于管理使用Java开发的交付件，后来逐步发展到可以支持更多领域。目前主流的开源方案是Nexus OSS和Artifactory。
