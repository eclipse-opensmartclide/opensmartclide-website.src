---
Title: A Simulation-Visualizer For Eclipse APP4MC
headline: "News"
date: 2021-02-03
categories: ["news"]
banner: "/images/news/GSoC-logo.png"
hide_sidebar: true
hide_breadcrumb: true
---

Philip Okonkwo, our guest author, was among the the students who have been accepted into the Google Summer of Code (GSoC) 2020 program. The exercise ended in September 2020 and he was one of those who successfully completed their chosen project on time and received a certificate of completion from Google. Like every GSoC project, the first step was to write a proposal that describes what the participant would like to contribute to the open source project. Philips proposal was about extending the capabilities of Eclipse APP4MC, which is one of the many open source projects managed by the Eclipse Foundation:

My 2020 Google Summer of Code included a project to create a simulation visualizer for Eclipse APP4MC. More specifically, the project goal was to visualize the execution trace of a simulated APP4MC model including the application's states using a framework such as Nebula Timeline. Henceforth, the scope lied in implementing a rudimentary simulation engine and a front-end for visualizing the results. The rudimentary simulation back-end should support a simple scheduling algorithm, such as fully preemptive fixed priority (FPFP) based scheduling. In the end I was able to implement an Earliest Deadline First Scheduler and a Rate Monotonic Scheduler in a Discrete Event Simulator as well as a SWT-based front-end interface for visualizing the execution traces on any partitioned Amalthea model in Eclipse APP4MC.

In detail my contributions consisted of the following aspects:

- Extending the Eclipse Nebula timeline widget to include the possibility of adding annotations that indicate arrival time and deadlines of tasks in the timeline view.
- Creating a user interface for visualizing the simulation trace.
- Implementing the simulation back-end by creating rudimentary schedulers, in particular Earliest Deadline First (EDF) and Rate Monotonic (RM) scheduling.
- Creating a visualization of the simulation of APP4MC models by connecting the model to the simulation back end and rendering the results on the GUI.
- Testing and documentation.

The project not only helped me to acquire new knowledge, but also deepened some of the skills I already had and fostered their application in real-world examples, such as

- Understanding and implementing the concepts of Discrete Event Simulation.
- A better understanding of the Amalthea model.
- The skills to develop software and use the tools available in the Eclipse Tool Platform, as I was not familiar with Eclipse and usually relied on other frameworks in the past.

My experience with the GSoC program is certainly something I approve of. There were set targets and goals for each specific phase of the program which made me able to plan my time well and incrementally add the features needed. The mentors are also available to help. I was lucky to have mentors who were always available to help and give insights especially in the areas of the tooling I was not familiar with. This saved a considerable amount of frustration and helped me advance quicker. I have contributed to open source in the past by adding little features and documentation to different open source projects but this was the first time I got to work on a full functionality myself as part of an open source project that will be used by many organizations and individuals.

The Google Summer of Code program is definitely something I would like to participate again if I get the chance especially if the organization I chose to work with is the Eclipse Foundation. I will advise anyone who wants to participate to endeavor to work and build some few projects in a programming language and stack that they will like to use and contribute to. This helps in estimating properly how much time and effort it would take to finish a task and thus be able to plan and manage time appropriately.

Finally, I'd like to conclude with a short animation of my work in action.

<img class="img-responsive" alt="Simulation Visualizer in action" src="/images/news/finalresult.gif">


<div class="bottomitem margin-bottom-20">
  <h3 class="header-underline">About the Author</h3>
  <div class="row">
    <div class="col-sm-24">
    	<div class="row">
        <div class="col-sm-6">
          <img class="img-responsive" width=200 alt="Philip Okonkwo" src="/images/news/philip.png"">
        </div>
        <div class="col-sm-16">
          <p class="author-name"><b>Philip Okonkwo</b></p>
          <p class="author-bio">Philip Okonkwo is a software developer with four years of experience in developing mobile and web applications with frameworks and languages like Android/Java, Flutter/Dart, Javascript and Django/Python. He gained experience by contributing to open source technologies like Google Flutter SDK. Besides coding, he likes to write short tutorials on Medium. Philip is currently pursuing his Masters degree in Embedded Systems for Mechatronics at the University of Applied Sciences and Arts, Dortmund.
		    </p>
        </div>
      </div>
    </div>
  </div>
</div>
