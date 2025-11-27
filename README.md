# Containers Workshop JJS

Here lie all the files you need to build a small, reproducible, Apptainer container.
This container will embed a notebook, as well as a Python environment to run it, and a standalone code, xtb, to do extra computation.

First, you should run 
```bash
apptainer help
```
To get the list of all available commands.
As an end user, the more relevant commands are: *build, exec, inspect, pull, run, run-help & shell*


To begin, we will need to build the container's image.
Using Apptainer, the command is
```bash
apptainer build [image-name].sif [container-definition].def
```

**[Text] are placeholders for the name you want/of the file.**

This can take a bit of time, as it needs to download and compile every piece of software needed.
You can benefit from this time to read and try to understand the definition file. More information on the different sections [here](https://apptainer.org/docs/user/main/definition_files.html)


When it's done, you can first try to *inspect* the image to display some metadata.
You can also try to *run-help* to see meaningful information on how to use it.

```bash
apptainer [inspect|run-help] .def 
```

This should give you enough information for what's left.
