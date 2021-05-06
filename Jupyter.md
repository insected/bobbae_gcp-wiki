
The [IPython](https://ipython.org) Notebook is now known as the Jupyter Notebook. 



[Jupyter](https://jupyter.org/) is an interactive computational environment, in which you can combine code execution, rich text, mathematics, plots and rich media.

The name “Jupyter” is a strong reference to Galileo, who detailed his discovery of the Moons of Jupiter in his astronomical notebooks. 

The name “Jupyter” is also a play on the languages Julia, Python, and R, which are pillars of the modern scientific world. 

[JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) is a web-based interactive development environment for Jupyter notebooks, code, and data.



There are several ways to run Jupyter notebooks in GCP. [AI Platform](https://cloud.google.com/ai-platform-notebooks), [Datalab](https://cloud.google.com/datalab/docs/how-to/working-with-notebooks), [Dataproc](https://cloud.google.com/dataproc/docs/concepts/components/jupyter), and [Colab](Colab) all support [Jupyter notebooks](https://www.youtube.com/watch?v=Eu57QKNHaiY). You could also create a [GCE](https://cloud.google.com/compute) [VM](VM) and install [Jupyter notebook manually](https://www.datacamp.com/community/tutorials/google-cloud-data-science) or use [terraform to provision a AI Platform Jupyter Notebook via Cloud Shell](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/notebooks_instance).  You can also [start Jupyter notebook servers on Google Kubernetes Engine](https://cloud.google.com/architecture/spawning-notebook-servers-on-gke-tutorial).
You can [create Jupyter Classroom environment with Google Container Engine](https://github.com/GoogleCloudPlatform/gke-jupyter-classroom).
The [Tensorflow and Jupyter](https://cloud.google.com/docs/tutorials#tensorflow+jupyter) can be used together. 



## Jupyter tips & tricks 

[https://www.youtube.com/watch?v=2eCHD6f_phE](https://www.youtube.com/watch?v=2eCHD6f_phE)


## Jupyter Kubeflow notebooks

[https://www.youtube.com/watch?v=eEsfPL6SvJc](https://www.youtube.com/watch?v=eEsfPL6SvJc)


[[https://cloud.google.com/architecture/images/spawning-notebook-servers-on-gke-tutorial-architecture.svg]]





## JupyterHub

With [JupyterHub](https://github.com/jupyterhub/jupyterhub) you can create a multi-user Hub which spawns, manages, and proxies multiple instances of the single-user Jupyter notebook server.
JupyterHub allows users to interact with a computing environment through a webpage. As most devices have access to a web browser, JupyterHub makes it is easy to provide and standardize the computing environment for a group of people (e.g., for a class of students or an analytics team).



Helm Chart & Documentation for [deploying  JupyterHub on Kubernetes](https://github.com/jupyterhub/zero-to-jupyterhub-k8s/).




