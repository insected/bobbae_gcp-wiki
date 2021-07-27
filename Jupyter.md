
[Jupyter Notebook]( https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook ) is based on 
[IPython](https://ipython.org) 


[Jupyter](https://jupyter.org/) is an interactive computational environment, in which you can combine code execution, rich text, mathematics, plots and rich media.

The name “Jupyter” is a  reference to Galileo, who detailed his discovery of the Moons of Jupiter in his [astronomical notebooks](https://www.nature.com/articles/31049). 
The name “Jupyter” is also a play on the languages [Julia](https://julialang.org/  ), Python, and [R](https://www.r-project.org/ ), which are pillars of the modern scientific world. 
[JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) is a web-based interactive development environment for Jupyter notebooks, code, and data.


There are many ways to run Jupyter notebooks in GCP: [Vertex AI Notebook](https://cloud.google.com/vertex-ai/docs/general/notebooks ), [AI Platform](https://cloud.google.com/ai-platform-notebooks), [Datalab](https://cloud.google.com/datalab/docs/how-to/working-with-notebooks), [Dataproc](https://cloud.google.com/dataproc/docs/concepts/components/jupyter), and [Colab](Colab) all support [Jupyter notebooks](https://www.youtube.com/watch?v=Eu57QKNHaiY). You could also create a [GCE](https://cloud.google.com/compute) [VM](VM) and install [Jupyter notebook manually](https://www.datacamp.com/community/tutorials/google-cloud-data-science) or use [terraform to provision a AI Platform Jupyter Notebook via Cloud Shell](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/notebooks_instance).  You can also [start Jupyter notebook servers on Google Kubernetes Engine](https://cloud.google.com/architecture/spawning-notebook-servers-on-gke-tutorial).
You can [create Jupyter Classroom environment with Google Container Engine](https://github.com/GoogleCloudPlatform/gke-jupyter-classroom).
[Tensorflow and Jupyter](https://cloud.google.com/docs/tutorials#tensorflow+jupyter) can be used together. You can use [Dataproc Hub](https://cloud.google.com/blog/products/data-analytics/administering-jupyter-notebooks-for-spark-workloads-on-dataproc ) to combine Jupiter Notebooks with ML, Spark and Hadoop based data lakes and open source data solutions.



## Jupyter tips & tricks 

[https://www.youtube.com/watch?v=2eCHD6f_phE](https://www.youtube.com/watch?v=2eCHD6f_phE)


## Jupyter Kubeflow notebooks

[https://www.youtube.com/watch?v=eEsfPL6SvJc](https://www.youtube.com/watch?v=eEsfPL6SvJc)


[[https://cloud.google.com/architecture/images/spawning-notebook-servers-on-gke-tutorial-architecture.svg]]





## JupyterHub

With [JupyterHub](https://github.com/jupyterhub/jupyterhub) you can create a multi-user Hub which spawns, manages, and proxies multiple instances of the single-user Jupyter notebook server.
JupyterHub allows users to interact with a computing environment through a webpage. As most devices have access to a web browser, JupyterHub makes it is easy to provide and standardize the computing environment for a group of people (e.g., for a class of students or an analytics team).



Helm Chart & Documentation for [deploying  JupyterHub on Kubernetes](https://github.com/jupyterhub/zero-to-jupyterhub-k8s/).




