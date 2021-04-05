# Contributing Guidelines

Thank you for your interest in contributing to our project. Whether it's a bug report, new feature, correction, or additional
documentation, we greatly value feedback and contributions from our community.

Please read through this document before submitting any issues or pull requests to ensure we have all the necessary
information to effectively respond to your bug report or contribution.


## Reporting Bugs/Feature Requests

We welcome you to use the GitHub issue tracker to report bugs or suggest features.

When filing an issue, please check existing open, or recently closed, issues to make sure somebody else hasn't already
reported the issue. Please try to include as much information as you can. Details like these are incredibly useful:

* A reproducible test case or series of steps
* The version of our code being used
* Any modifications you've made relevant to the bug
* Anything unusual about your environment or deployment


## Contributing via Pull Requests
Contributions via pull requests are much appreciated. Before sending us a pull request, please ensure that:

1. You are working against the latest source on the *main* branch.
2. You check existing open, and recently merged, pull requests to make sure someone else hasn't addressed the problem already.
3. You open an issue to discuss any significant work - we would hate for your time to be wasted.

To send us a pull request, please:

1. Fork the repository.
2. Modify the source; please focus on the specific change you are contributing. If you also reformat all the code, it will be hard for us to focus on your change.
3. Ensure local tests pass.
4. Commit to your fork using clear commit messages.
5. Send us a pull request, answering any default questions in the pull request interface.
6. Pay attention to any automated CI failures reported in the pull request, and stay involved in the conversation.

GitHub provides additional document on [forking a repository](https://help.github.com/articles/fork-a-repo/) and
[creating a pull request](https://help.github.com/articles/creating-a-pull-request/).

## Adding an Example

Any new example must be added in the `examples` directory.
When adding a new example, there are several things to consider as you implement:

### Added Value
As an official learning resource, it is important that any new examples add value to our learning resources. This means that it should not duplicate an existing example.

### Introduction Structure

* The example must have a descriptive `file name` and `title` that clearly defines it’s usage and the `topics` that it would cover. Follow a file naming pattern - feature/function`-`app/lib.ipynb
* The example must have a `Prerequisites` markdown that lists the installations required before executing the notebook as is attached to a cluster. For eg: EMR applications required like Hive, Presto, etc.
* The example must have an `Introduction` markdown that explains the basics of the topics covered in the notebook. The introduction should include links to relevant aws public docs and data sets used in the notebook.
* Every `code cell` must be preceded by a `markdown cell` that clearly explains the following code cell in detail and provides any additional usage or information.
* Text portions of notebooks should follow the [AWS Style Guide](https://alpha-docs-aws.amazon.com/awsstyleguide/latest/styleguide/Welcome.html) and guidelines for [service names](https://w.amazon.com/bin/view/AWSDocs/editing/service-names/).
* Assume only the knowledge that a beginner data scientist would have. Don’t assume that the reader is an experienced coder or has a rigorous technical background.

### Code Cells Structure

* The example should not contain any sensitive information like security groups/subnets, passwords, etc in any of the code or markdown cells.
* The kernel that you use to write your notebook must be named exactly the same as one of the default kernels that ships with EMR notebooks. The best way to avoid this problem is to actually author your notebook file within a EMR Notebook.
* It's preferred that the cell outputs be left empty. Use `Edit` and `Clear All` before submitting a PR.

### Testing
The example must be tested using an EMR Notebook and should have successfully run when attached to a cluster.

### Style and Formatting
We strive to keep all the examples consistent in style and formatting and as idiomatic as possible. This hopefully makes navigating examples easier for users.


## Finding contributions to work on
Looking at the existing issues is a great way to find something to contribute on. As our projects, by default, use the default GitHub issue labels (enhancement/bug/duplicate/help wanted/invalid/question/wontfix), looking at any 'help wanted' issues is a great place to start.


## Code of Conduct
This project has adopted the [Amazon Open Source Code of Conduct](https://aws.github.io/code-of-conduct).
For more information see the [Code of Conduct FAQ](https://aws.github.io/code-of-conduct-faq) or contact
opensource-codeofconduct@amazon.com with any additional questions or comments.


## Security issue notifications
If you discover a potential security issue in this project we ask that you notify AWS/Amazon Security via our [vulnerability reporting page](http://aws.amazon.com/security/vulnerability-reporting/). Please do **not** create a public github issue.


## Licensing

See the [LICENSE](LICENSE) file for our project's licensing. We will ask you to confirm the licensing of your contribution.
