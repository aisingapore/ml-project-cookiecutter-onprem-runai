# Prerequisites

## Software & Tooling Prerequisites

Aside from an internet connection, you would need the following to
follow through with the guide:

- NUS Staff/Student account.
- Azure account provisioned by AI Singapore.
- PC with the following installed:
    - If your machine is with a Windows OS, use
      [__PowerShell__](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.2)
      instead of the default Command (`cmd.exe`) shell. Best if you
      resort to
      [Windows Terminal](https://docs.microsoft.com/en-us/windows/terminal/).
    - __Pulse Secure__
        - Refer to [NUS IT eGuides](https://nusit.nus.edu.sg/eguides/)
          for installation guides.
    - __Web browser__
    - __Terminal__
    - __[Git](https://git-scm.com/downloads)__
    - __[Rancher Desktop](https://rancherdesktop.io)__ or
      __[Docker Engine](https://docs.docker.com/engine/install):__
      Client-server application for containerising applications as well
      as interacting with the Docker daemon.
        - For Linux users, you may install the Docker Engine (Docker daemon)
          directly.
        - For Windows or macOS users, the Docker daemon can be installed
          through [Rancher Desktop](https://rancherdesktop.io).
    - __[miniconda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html):__
      for Python virtual environment management.
    - __[`kubectl`](https://kubernetes.io/docs/tasks/tools/):__
      CLI for Kubernetes.
    - *(Optional)* __[`helm`](https://helm.sh/docs/intro/install/):__
      CLI for Kubernetes' package manager.
- Access to a project on AI Singapore's Run:ai cluster.
  See [here](./03-mlops-components-platform.md#runai) for more information.
- Credentials for AI Singapore's Elastic Cloud Storage (ECS) service.
  See [here](./03-mlops-components-platform.md#elastic-cloud-storage-ecs) for more information.
- Credentials for AI Singapore's Harbor registry.
  See [here](./03-mlops-components-platform.md#harbor) for more information.
- Credentials for an MLflow Tracking server.
  See [here](./03-mlops-components-platform.md#mlflow) for more information.

!!! note
    If you do not have any of the required credentials,
    please verify with or notify the MLOps team at
    `mlops@aisingapore.org`.

!!! info
    Wherever relevant, you can toggle between the different commands
    that need to be executed
    for either Linux/macOS or the Windows environment (PowerShell).
    See below for an example:

    === "Linux/macOS"

        ```bash
        # Get a list of files/folders in current directory
        $ ls -la
        ```

    === "Windows PowerShell"

        ```powershell
        # Get a list of files/folders in current directory
        $ Get-ChildItem . -Force
        ```

    !!! caution
        If you are on Windows OS, you would need to ensure that the
        files you've cloned or written on your machine be with
        `LF` line endings. Otherwise, issues would arise when Docker
        containers are being built or run. See
        [here](https://stackoverflow.com/questions/48692741/how-can-i-make-all-line-endings-eols-in-all-files-in-visual-studio-code-unix)
        on how to configure consistent line endings for a whole folder
        or workspace using VSCode.