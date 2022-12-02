---
Title: "BTF (Best Trace Format) generation on RTFParallella (Real Time Framework Parallella)"
headline: "News"
date: 2021-01-25
categories: ["news"]
banner: "/images/news/GSoC-logo.png"
hide_sidebar: true
hide_breadcrumb: true
---

Our guest author Anand Prakash was among the the students who have been accepted into the Google Summer of Code (GSoC) 2020 program. He is pleased to share his experience and learning from the Google Summer of Code (GSoC) project that he successfully completed in September 2020:

My proposal was accepted for GSoC 2020 by the Eclipse APP4MC committers on behalf of the Eclipse Foundation. The title of my proposal was BTF (Best Trace Format) generation on RTFParallella (Real Time Framework Parallella). In particular, the project involved implementing tracing framework based on the BTF specification over the existing RTFParallella Framework. The Adapteva Parallella development board was used as the hardware platform in order to enable a tracing based real-time analysis of an Amalthea model. It included establishing timing synchronization between the host ARM processor and Epiphany 16-core co-processor. The tick count used for tracing the task state was replaced with the actual timestamp values. The time scaling factor was also made configurable based on user specified data. The tracing framework on RTFParallella is developed in C, and the generated BTF trace file can be viewed on visualization tools such as Eclipse Trace Compass for evaluation purpose.

Another aspect of the project was to enhance the capabilities of the code generation tooling in order enable synthesizing executable code with proper tracing extensions for any given Amalthea Model. The implementation to include the tracing functionality into the code generator was developed in Java.

The project was completed within the specified time frame with the following deliverables:

- Source code changes consisting of BTF trace framework on RTFParallella.
- Source code changes for feature enhancement of the code generator to automatically synthesize the tracing functionality.
- API Documentation and User Manual.

![Workflow for generating traces using RTFParallella](/images/news/datapath_flow.png)

The figure above depicts the typical workflow for generating trace information out of an Amalthea model. The CdGen code generator synthesizes executable code that is compiled and ran on a hardware platform in order to generate a BTF trace file. For the sake of visualization and assessment, the resulting trace can be inspected in tools such as Eclipse Trace Compass. An example of a trace's visualization using Eclipse Trace Compass is illustrated below.

![Example Trace visualized with Eclipse Trace Compass](/images/news/trace_output.png)

The activities related to GSoC were a valuable learning experience that allowed me to foster the following technical skills:

- Gained knowledge on multi-core and many core processor architecture.
- Enhanced my understanding on inter-process communication.
- Gained experience in implementing resource sharing techniques.
- Better understanding of distributed and shared memory architecture.
- Task model based on OSEK architecture.
- Experience in realization of Amalthea model on actual hardware.
- Understanding of BTF specification and its usage in event tracing.
- Real-time Analysis of Amalthea task model simulation.

In terms of organizational learning, GSoC dedicated an ample amount of time for community bonding during which we learned about the open source organization, the ongoing projects and their way of working. It provided an opportunity to interact with mentors and discuss possible ideas regarding the GSoC project. It provided me an insight about how my contribution will affect the overall project. Certain terminologies such as Contributor, Committer which are frequently used in open source community was a good learning for me. I also gained insight on the review and integration process of committing code to an open source repository.

Overall, my experience during the GSoC project has been really good. The program itself is very streamlined with allocated and fixed deadlines for each phase of the project. This helped me in planning my task and work load in advance which made the project less stressful. Reviews are done at the end of each phase which also helps in understanding the expectations, scope and quality of work required to complete the project. I appreciated the considerable freedom I had in terms of certain decisions during my GSoC project. Besides it provided me a platform to contribute to an open source which is highly appreciated in industry and is good for personal exposure. Overall, my expectations were met by the end of the project.

As a general advice, I'd like to point out that GSoC projects need self-discipline and self-motivation. It is a testament of how passionate you are about programming. It reflects your work ethics and at the same time provide you an opportunity to improve your software architecture design and coding skills. You learn every aspect of a project right from formulating a proposal, to design, code, test and documentation of your work. Therefore, I would highly recommend any programming enthusiast to experience this amazing opportunity offered by Google and supported by the Eclipse Foundation.

<div class="bottomitem margin-bottom-20">
  <h3 class="header-underline">About the Author</h3>
  <div class="row">
    <div class="col-sm-24">
      <div class="row margin-bottom-20">
        <div class="col-sm-6">
           ![Anand Prakash](/images/news/anand.png)
        </div>
        <div class="col-sm-16">
          <p class="author-name"><b>Anand Prakash</b></p>
          <p class="author-bio">Anand is pursuing his master’s at Fachhochschule Dortmund in Embedded Systems for Mechatronics. Besides his studies, he is working as a student assistant at IDIAL Institute under project PANORAMA. Prior to joining the Master programme, Anand worked as a Software Engineer in companies involving the Display industry and Smart Card domain. He is proficient in programming languages such as C and worked extensively in security algorithms. He also has knowledge on working on different Operating System platform. 
          The GSoC program at Fachhochschule  Dortmund gave him an opportunity to work on heterogeneous platform such as Adapteva Parallella and contributing to open source. Implementation of tracing framework based on BTF specification was quite challenging. At the same time, it gave him an experience and understanding of distributed and shared memory architecture.
		    </p>
        </div>
      </div>
    </div>
  </div>
</div>
