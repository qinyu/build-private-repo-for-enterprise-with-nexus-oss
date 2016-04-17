# 方案

本方案选择了相对成熟的Nexus OSS。Nexus OSS目前已经发布3.0版本，相对于2.12版本来说，最大的变化是增加了对Docker Hub私服的支持，可以根据自己的需要选择相应的版本。

关于Nexus OSS的介绍，安装，配置等基本操作，请参考[Nexus官方文档](http://books.sonatype.com/nexus-book/reference/)。

如果是千人以下的开发团队，一台Nexus OSS已经足够支撑所有使用。但对于大型企业来说：
1. 内部交付件是核心财富，必须妥善存储
2. 内部交付件往往是其他团队开发构建必须依赖的基础组件，私服必须随时提供拉取服务。

这就要求方案必须提供高可用性。Nexus OSS有篇关于如何构建高可用私服的[博客](http://www.sonatype.org/nexus/2015/07/10/high-availability-ha-and-continuous-integration-ci-with-nexus-oss/)。

本方案根据此博客设计，并作了一定扩展，形成了简化版和高级版两个方案。企业可以根据成本以及需要服务的团队数量灵活调整。

除了根据设计部署相应的服务，团队还必须用一套良好的管理机制，维护方法以及应急方案，并加以贯彻执行，才能保障服务的可靠性。
