# 11.1 Warming up
Think about a hypothetical situation where we have an application being worked on by a team of about 6 people. The application is in active development and will be released soon.

Let us assume that the application is coded with some other language than JavaScript/TypeScript, e.g. in Python, Java, or Ruby. You can freely pick the language. This might even be a language you do not know much yourself.

Write a short text, say 200-300 words, where you answer or discuss some of the points below. You can check the length with https://wordcounter.net/. Save your answer to the file named exercise1.md in the root of the repository that you shall create in exercise 11.2.

The points to discuss:

- Some common steps in a CI setup include linting, testing, and building. What are the specific tools for taking care of these steps in the ecosystem of the language you picked? You can search for the answers by Google.
- What alternatives are there to set up the CI besides Jenkins and GitHub Actions? Again, you can ask Google!
- Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?


Remember that there are no 'right' answers to the above!

## Answer

Let's say the development is in Python. 
- One linting tool is [Pylint](https://github.com/pylint-dev/pylint). For testing, the standard library has unittest, and one decent community testing library is [pytest](https://github.com/pytest-dev/pytest). As mentioned in the material, Python isn't really built per-say, but I guess the closest to how compiled languages are "built", namely compiled into an executable binary file, is something like [PyInstaller](https://github.com/pyinstaller/pyinstaller) or [cx_Freeze](https://github.com/marcelotduarte/cx_Freeze), for example.
- Plenty of tools for this, I reckon. One example is Atlassian's [Bitbucket Pipelines](https://www.atlassian.com/software/bitbucket/features/pipelines), and Gitlab have their [own stuff](https://docs.gitlab.com/ee/ci/), to compare with Github Actions.
- The last point is also discussed already in the material. As mentioned, the choice of environment depends on the project. Self-hosted is naturally better if you want more control of the environment or want to keep the project more private. Cloud-based setups are presumably generally easier to setup and manage, especially as the user does not need to worry about the hardware, so if the project is quite simple, it's probably better to go for that. Simply put, determine the requirements for the project, and if a cloud-based solution suffices, go for that, and if something more is needed, a self-hosted setup would be the choice.