# Generic app architecture

**Table of content:**
- [Wings of software architecture](#item-sw-arch)
- [App development paradigm](#item-one)
- [Cloud Architecture front block](#front-block)
- [Web Application backend](#item-two)
- [Hosted Web Applicaiton](#item-three)
- [Scaling](#scaling)

\
<br/>


<a id="item-sw-arch"></a>
### Wings of software architecture

<img src="techpages/archsnapshots/ArchitectureDoc.png?raw=true"/>


\
<br/>

<a id="item-one"></a>
### App development

<img src="techpages/archsnapshots/AppDev.png?raw=true"/>

\
<br/>
<a id="front-block"></a>
### Cloud architecture front block

<img src="techpages/archsnapshots/CloudArchFrontBlock.png?raw=true"/>

\
<br/>

<a id="item-two"></a>
### Web Application backend

<img src="techpages/archsnapshots/SampleWebAppBackend.png?raw=true"/>

\
<br/>

<a id="item-three"></a>
### Hosted Web Application

<img src="techpages/archsnapshots/SampleWebApp.png?raw=true"/>

\
<br/>

<a id="scaling"></a>
## Scalability
<br/>

1. Horizontal Scaling, Scaling out
2. Vertical Scaling, Scaling up

<br/>
####App design time
<br/>

|                 | Vertical scaling                                       | Horizontal scaling   |
|-----------------|--------------------------------------------------------|---------------------------------------|
|Application logic| Functional decomposition, Scale by splitting components| Performance optimization, app thinning|
|App data         | Streaming data, Chunked encoding                       | nvarchar-to-Object Storage            |

<br/>
####App runtime
<br/>

|              | Vertical scaling                            | Horizontal scaling               |
|--------------|---------------------------------------------|----------------------------------|
|Infrastructure|Auto-scale nodes, VMs, Elastic database pools| Compute capacity, Memory, Storage|
|App data      |Data partiioning, sharding                   | Elastic storage                  |

<br/>
### Scale cube

  * *x-axis*: Scale by cloning server instances
  * *y-axis*: Scale by functional decomposition of application
  * *z-axis*: Scale by data partitioning with multiple instances working with exclusive data sets


<br/>
