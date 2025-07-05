The team will be using Python. 

When it comes to a linting tool that can be used in a CI setup, Ruff from Astral seems to be the most popular option. It is both a formatter and a linter. Alternatively, pylint, black, and uv are other viable options.

For a testing tool in a CI setup, pytest seems to be a common and well-used third-party library. The standard library also has the unittest module which works for testing. PyUnit also seems to be another viable option as it it heavily inspired by JUnit which is used for Java testing.

Since Python is interpreted, build tools are often not necessary. However, if there is a pre-compilation step required, some viable build tools include: PyBuilder, Poetry, doit, invoke, among others.

Some popular options for CI alternatives include Travis CI, GitLab CI, TeamCity and Space, Drone CI, among others.

For this particular setup, since there are only 6 people working on this project, they most likely do not need the customizability, flexibility, and scalability of a custom server CI setup. Of course, it depends on what the project is and what the requirements are for the project. Does this project need to use a graphics card to run tests? Will this project be computationally demanding and need to choose more powerful machines on demand? Can this project afford to spend time and money on setting up and configuring a custom CI/CD and getting its developers up to speed on a complex tool like Jenkins? This is the kind of information that is needed to make this decision. Usually, smaller teams prioritize building features, getting to market, and may not want to deal with configuration. Performance might be worse on a cloud-based environment, but this project may not demand ample computational resources. Instead, a cloud-based environment would probably suit their needs unless they have "special" needs.