# CheckPoint SourceGuard
Check Point Software SAST source code and container image scanner

With the rapid adoption of devops for application build and runtime, workloads have evolved from infrastructure servers and virtual machines to code with containers and serverless.
Infrastructure style security has to evolve as well to code centric security from application build to runtime by shifting to the left and by becoming treated as code.
DevOps is built around a CI/CD methodology with various stage where all the stages are automated and interconnected by pipeline from build to deployment.
For the application of security in an CI/CD pipeline, it is important to identify the stages of the CI/CD pipeline. 
This is well illustrated by the 4Cs of Cloud Native Security as defined by the CNCF. 
The 4Cs encompass code,container,kubernetes(COE) and Cloud(hybrid, multi, private,on-prem) and are depending on each other. Securing each element of the 4Cs is critical.
https://kubernetes.io/docs/concepts/security/overview/
           
   ![header image](https://github.com/dean-houari/Mastering-Kubernetes/blob/master/LAB/4c.png)
   
The first stage when the application developpers is to upload sourcen code to a various branches to a versioned repository such GitHub or Git. In order to ensure that the code is secure and free of potential source of attacks such as credentials
and CVEs, it is important to perform source code scanning statically and dynamically identified as SAST and DAST. Effectively scanning when it is ready and commited to a branch and while it is being stored
in a branch on a repo.
When the code is ready to be compiled into an artifact such as a container, it is important to then scan the container image to tested and deployed.
We will be providing support for Docker and the way to create a container is with a Dockerfile which defines the containers images, source code and commands used by the app container image.
As developpers get these container images such as busybox, node, nginx etc.. from DockerHub, they may be including CVEs and critical malware.
The SourceGuard scanner will provide SAST and DAST for source code and container images. 
there are many SAST and DAST scanners such Clair and Anchore but the true se3curity value is with the ability to find CVEs and Critical Malware.
We at CheckPoint will be using ThreatCloud on the scanner backend. ThreadCloud is the market leading vulnerability and CVE DB that is been succesfully used
on our endpoint security.
ThreatCloud will bring the best CVE and Malware DBs engine with our SAST and DAST security. 
SourceGuard is in available for Beta testing on the CheckPoint Infinity portal.

## SourceGuard Installation

Please go to portal.checkpoint.com 
Create an account by signing up to Infinity even if you are a checkpoint employee. The default space for checkpoint employee is cp-all-demo which cannot be used.

   ![header image](infinity1.png)
   
   


