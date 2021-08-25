This folder is part of the Docker context.
Taken directly from the apache airflow git.


Most of other folders in Airflow are not part of the context in order to make the context smaller.

The Production [Dockerfile](../Dockerfile) and the CI one [Dockerfile.ci](../Dockerfile.ci) copies
the [docker-context-files](.) folder to the image context - in case of production image it copies it to
the build segment, co content of the folder is available in the `/docker-context-file` folder inside
the build image. You can store constraint files and wheel
packages there that you want to install as PYPI packages and refer to those packages using
`--constraint-location` flag for constraints or by using `--install-from-docker-context-files` flag.

By default, the content of this folder is .gitignored so that any binaries and files you put here are only
used for local builds and not committed to the repository.