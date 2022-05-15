# Work Sample for Data Aspect, Pandas Variant

[What is this for?](https://github.com/EQWorks/work-samples#what-is-this)

## Environment setup

If you already have a functioning Python and Pandas configuration, you can use your own. For your convenience, the provided `docker-compose.yml` is based on the [`jupyter/scipy-notebook`](https://github.com/jupyter/docker-stacks/tree/master/scipy-notebook) image. You will need to have Docker and Docker Compose configured on your computer. Check out the [Docker Desktop documentation](https://docs.docker.com/desktop/) for details.

You can run `docker-compose up` and follow the prompt to open the Jupyter Notebook UI (looks like `http://127.0.0.1:8888/?token=<SOME_TOKEN>`).

The given `data/` directory mounts as a Docker volume at `~/data/` for easy access:

```python
import os
import pandas as pd

df = pd.read_csv(os.path.expanduser('~/data/DataSample.csv'))
```

![example](https://user-images.githubusercontent.com/2837532/110395836-e8610e80-803c-11eb-92fe-2891e06a1b97.png)

## Submission

Please host your solution as one or multiple Notebooks (`.ipynb`) in a public git remote repository and reply with its link to the email thread you initially received to work on this work sample.
