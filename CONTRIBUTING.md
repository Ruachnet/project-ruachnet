# Contributing to Hyperledger Besu
## :tada: Thanks for taking the time to contribute! :tada:

Welcome to the Besu repository! The following links are a set of guidelines for contributing to this repo and its packages. These are mostly guidelines, not rules. Use your best judgement, and feel free to propose changes to this document in a pull request. Contributions come in the form of code submissions, writing documentation, raising issues, helping others in chat, and any other actions that help develop Besu.

### Github/Discord/LF Accounts

Having the following accounts is necessary for contributing code/issues to Besu.  
* If you want to contribute code, you can make a [github account here](https://github.com).  
* If you want to raise an issue, do so [in the issues tab](https://github.com/Ruachnet/project-ruachnet/issues).
* To ask questions or chat with us, join our [Discord](https://discord.gg/Mjup2t8G)
* To edit pages in our wiki, you'll need a [Linux Foundation (LF) account].

# Contributing to Ruachnet

We’re excited that you’re interested in contributing to Ruachnet!
This document provides guidance on how to get started, the contribution workflow, and the community practices we follow.  

For **quick questions or sensitive matters**, please reach us via the **official email listed on the Ruachnet GitHub profile**.

---

## Useful Contributing Links

- [I just have a quick question](mailto:<ruachnet254@gmail.com>)  
- [How to Contribute](#-how-to-contribute)  
- [First Contribution Workflow](#-first-contribution-workflow)  
- [Did you find a bug?](mailto:<ruachnet254@gmail.com>)  
- [Issues](https://github.com/Ruachnet/project-ruachnet/issues)  
- [DCO (Developer Certificate of Origin)](https://developercertificate.org/)  
- [Suggesting Enhancements](mailto:<ruachnet254@gmail.com>)  
- [Pull Requests](https://github.com/Ruachnet/project-ruachnet/pulls)  
- [Code Reviews](#-code-reviews)  
- [Security Contributions](mailto:<ruachnet254@gmail.com>)  

---

## How to Contribute

There are many ways you can contribute to Ruachnet:

- **Report bugs** → Send details via email or open an issue.  
- **Propose enhancements** → Share ideas that could improve the project.  
- **Write code** → Submit pull requests with bug fixes, new features, or documentation improvements.  
- **Review code** → Provide feedback on open pull requests.  
- **Improve documentation** → Fix typos, clarify instructions, or add tutorials.  

Before contributing code, ensure you:  
1. Sign off your commits according to the **DCO**.  
2. Follow the project’s coding style and guidelines.  
3. Engage respectfully following the **Code of Conduct**.  

---

## First Contribution Workflow

Here’s a step-by-step guide to making your first contribution:

1. **Fork the repository**  
   - Go to [Ruachnet GitHub](https://github.com/ruachnet/ruachnet) and fork the repo.  

2. **Clone your fork**  
   ```bash
   git clone https://github.com/<your-username>/ruachnet.git
   cd ruachnet
   ```
3.  **Create a new branch**
    ```bash
    git checkout -b feature/my-new-feature
    ```
4.  **Make your changes**
    Add code, fix bugs, or update documentation.
5.  **Commit with DCO sign-off**
    ```bash
    git commit -s -m "Add new feature"
    ```
6.  **Push changes**
    ```bash
    git push origin feature/my-new-feature
    ```
7. **Open a Pull Request**
    Go to your fork on GitHub and open a PR against the main branch of Ruachnet.

## Guidelines for Non-Code and other Trivial Contributions
### Code Reviews

Code reviews are essential for maintaining quality. Here’s what we expect:

- **Be constructive** → Suggest improvements, not just problems.  
- **Be respectful** → Assume positive intent from contributors.  
- **Be specific** → Highlight exact lines or functions that could improve.  
- **Follow guidelines** → Ensure DCO, tests, and linting are in place before approval.  

Maintainers will merge PRs once they meet quality standards and align with the roadmap.  

---

#### Governance

Ruachnet is governed with openness and fairness.

- **Maintainers** are responsible for reviewing PRs, triaging issues, and ensuring project health.  
- **Contributors** are anyone who makes contributions (code, docs, or discussions).  
- **Decisions** are made through consensus whenever possible.  
- **Disagreements** should be resolved constructively—if unresolved, maintainers have final say.  
- **Becoming a maintainer** requires consistent and meaningful contributions over time.  

Please keep in mind that we do not accept non-code contributions like fixing comments, typos or some other trivial fixes. Although we appreciate the extra help, managing lots of these small contributions is unfeasible, and puts extra pressure in our continuous delivery systems (running all tests, etc). Feel free to open an issue pointing any of those errors, and we will batch them into a single change.

[How to Contribute]: https://wiki.hyperledger.org/display/BESU/How+to+Contribute
[Linux Foundation (LF) account]: https://identity.linuxfoundation.org/
