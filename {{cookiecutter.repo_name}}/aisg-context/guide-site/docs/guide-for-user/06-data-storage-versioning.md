# Data Storage & Versioning

## Sample Data

While you may have your own project data to work with, for the purpose
of following through with this template guide, let's download
the sample data for the
[sample problem statement](./02-preface.md#guides-problem-statement)
at hand.

!!! info
    The sample data for this guide's problem statement is made
    accessible to the public. Hence any team or individual can download
    it. It is highly likely that your project's data is not
    publicly accessible
    and neither should it be, especially if it is a 100E project.

=== "VSCode Server Terminal"

    ```bash
    $ mkdir -p /<NAME_OF_DATA_SOURCE>/workspaces/<YOUR_NAME>/data && cd "$_"
    $ unzip mnist-pngs-data-aisg.zip
    ```

In the next section, we will work towards processing this set of raw
data and eventually training an image classification model.