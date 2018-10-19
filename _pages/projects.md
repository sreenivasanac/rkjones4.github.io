---
title: ""
permalink: /projects/
toc: true
toc_label: "Projects"
toc_icon: "cog"
toc_sticky: true
---


# Machine Learning

## GANGogh

![music]( {{ "assets/images/gangogh_gif.gif"" | relative_url }})

*(2017 Independent research project supervised by [Andrea Danyluk](http://www.cs.williams.edu/~andrea/)).*
 
Generative Adversarial Networks are comprised of two deep neural networks pitted against one another in a zero-sum game. The aim of this project was to use GANs to generate novel pieces of art. The model was trained in tensorflow on a distribution of art pieces gathered from wikiart.org. Our architecture leveraged the power of the improved wasserstein metric in an extension of the typical AC-GAN framework that allowed us to condition our models on painting genre. In order to induce our generator to focus on learning the differences between genres, we additionally employed global conditioning and pre-training of the discriminator, which not only produced quality image samples in genres such as Flower Paintings and Landscapes, but also resulted in our discriminator outperforming the best literature accuracy values on the wikiart classification problem.


Blog | Code | Framework | Collaborator
--- | --- | --- | ---
 [Medium](https://towardsdatascience.com/gangogh-creating-art-with-gans-8d087d8f74a1) | [Github](https://github.com/rkjones4/GANGogh) | TensorFlow |  Derrick Bonafilia


## Music Genre Classification

![music]( {{ "assets/images/music_gif.gif"" | relative_url }})

*(2016 Machine Learning final project supervised by [Andrea Danyluk](http://www.cs.williams.edu/~andrea/)).* 

In this project, we approached the problem of music genre classification as an image-based classification task by transforming 30 second song snippets from the GTZAN dataset into spectrograms. Compared to previous approaches in this space, we did not transform our image into a set of dense-features, but rather fed our raw images into a simple convolutional neural network. Moreover, by treating each 30 second song as a collection of ten 3 second songs at training time, and implementing a voting mechanism over these 10 images at inference time, we were able to outperform most previous literature accuracy values on the GTZAN dataset. 

PPT | Framework | Collaborator
--- | --- | --- 
[Genre Classification](/assets/pdfs/genre.pdf) | TensorFlow | Derrick Bonafilia

## Facebook - Social Good ML

![sg]( {{ "assets/images/sg_gif.gif"" | relative_url }})

*(2017+ Facebook Machine Learning Engineer).* 

The Charitable Giving team at Facebook has a mission to foster a global community of giving. In this capacity, I’ve owned products that span from news feed, optimizing the distribution of our stories using prediction models, to natural language understanding tasks the center around inferring fundraiser creation intent. These projects have been responsible for over 25% of the teams total growth since I’ve joined the team, and have helped millions of people across the globe raise funds for the causes that matter to them. 

# Graphics

## Procedurally Generated Landscapes

![landscape]( {{ "assets/images/landscape_gif_real.gif"" | relative_url }})

*(2016 Graphics midterm project taught by [Morgan McGuire](https://www.cs.williams.edu/~morgan/)).*

The goal of this project was to procedurally generate unique stylized low-polygon worlds that evoked imagery of the Irish countryside. The terrain was produced through a series of operations on various cuts of perlin noise, which both seperated chunks of the world into different Biomes and produced the basis of the underlying mesh. To complete the stylized effect, we implemented a mesh simplification technique through point sampling based on the gradient of the terrain and triangulation methods. The final coloring of the mesh was based on a combination of Voronoi diagrams for the farmland and elevation and slope rules for the other Biomes. 

Report | Language/Framework | Collaborator(s)
--- | --- | ---
[Landscape Generation](https://www.cs.williams.edu/~morgan/cs371-f16/gallery/4-midterm/terrain/report.md.html) | C++/G3D | Melanie Subbiah, Yi-Tong Tseo, and Cole Erickson

## Simulating and Rending Water

![water]( {{ "assets/images/water_gif.gif"" | relative_url }})

*(2016 Graphics final project taught by [Morgan McGuire](https://www.cs.williams.edu/~morgan/)).* 

Our project was designed to both simulate and render realistic representations of water. The PBD particle simulation was backed by NVIDIA’s FleX engine, which output both locations of permanent water particles and transitory foam that was formed when neighboring particles had kinetic energies that surpassed a given threshold. With each iteration of the particle engine, surface meshes were re-generated using the marching cubes algorithm. The final rendering was done using path-tracing, and took into account Beer-Lambert coloring fake caustics, refraction, and reflection effects. 

Video | Code | Language/Framework | Collaborator(s) 
--- | --- | --- | -- 
[Water Video](https://www.youtube.com/watch?v=FS6nkQwO7pY) | [GitHub](https://github.com/YitongTseo/WaterSimulationAndRendering) | C++/G3D+Flex | Melanie Subbiah, Yi-Tong Tseo, and Cole Erickson

# Programming

## Encoding Information with Images and Memory

![valt]( {{ "assets/images/mindburnr_gif.gif"" | relative_url }})

*(2015 Summer Research Assistant working with [Brent Heeringa] (http://www.cs.williams.edu/~heeringa/)).*

 Collaborated with Nola Gordon in assisting Brent build out a prototype system for helping people remember sensitive information through error-sensitive encodings in recognizable images. Most of our work centered around building out multiple variants of the service in preparing mechanical turk experiments and generalizing some of the back-end infrastructure. Brent now leads [Valt](https://valt.io/), which is a company based on this line of investigation.

## Seam Carving

![sc]( {{ "assets/images/seamcarving_gif.gif"" | relative_url }})

*(2014 Data Structures final project taught by [Morgan McGuire](https://www.cs.williams.edu/~morgan/)).*

Implemented Avidan and Shamir’s Seam Carving Algorithm in C++. 

Report | Collaborator(s)
--- | ---
[Seam Carving](/assets/pdfs/carving.pdf) | Zijie Zhu, Julia Goldman, Yiheng Zhang

## Customized A/B Testing Framework

![d3]( {{ "assets/images/deltoid_gif.gif"" | relative_url }})

*(2016 SWE Intern at Facebook)*

Worked on the A/B testing platform [team](https://www.youtube.com/watch?v=Iw40wdwkkLA). Over the course of my internship, I worked full-stack (python, PHP/Hack, SQL) to build out a tool for ad-hoc statistical analysis of custom experiment data sets, and integrated that tool into the existing infrastructure. It’s still widely used by many data scientist at Facebook today.