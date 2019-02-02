# Containerize Applications

* Running your application in docker container
    * Create a image out of running continer (not recomended)
    * Dockerfile  (TextFile => INstructions)

* Dockerfile
   => INSTRUCTIONS
      =>
   => base image
       => scratch
   => configurations 

   FROM <baseimage>:<tag>
   RUN apt-get update&& apt-get install apache2-y

   * No instruction should ask prompts/question

* Process that happens

* Image name format is <registryname>/repository:<imagetag>


* Image is combination of layers stacked on each other and it will have a manifest




