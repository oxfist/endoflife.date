---
title: SonarQube
category: server-app
iconSlug: sonarqube
permalink: /sonar
alternate_urls:
-   /sonarqube
releasePolicyLink: https://www.sonarqube.org/downloads/lts/
changelogTemplate: "https://www.sonarqube.org/sonarqube-{{'__LATEST__'|split:'.'|pop|join:'-'}}/"
activeSupportColumn: true
releaseColumn: true
releaseDateColumn: true
eolColumn: Bug and Security Fixes

auto:
-   dockerhub: library/sonarqube
    regex: ^(?<major>\d+)\.(?<minor>\d+)\.(?<patch>\d+)-community$

releases:
-   releaseCycle: "9"
    releaseDate: 2021-07-02
    support: true
    eol: false
    latest: "9.8.0"
    latestReleaseDate: 2022-12-19

-   releaseCycle: "8"
    releaseDate: 2020-05-08
    support: 2021-07-05
    # Should be 2022-11-04 as per the policy, but is now in the past
    eol: false
    lts: 2021-05-04
    latest: "8.9.10"
    latestReleaseDate: 2022-12-19
    link: https://www.sonarqube.org/sonarqube-8-9-lts/

-   releaseCycle: "7"
    # https://groups.google.com/g/sonarqube/c/p3l3naFctpg/m/Sbk7fzX3AgAJ
    releaseDate: 2019-12-04
    support: 2019-10-16
    eol: 2021-05-04
    lts: 2019-07-01
    latest: "7.9.6"
    latestReleaseDate: 2021-04-22
    link: https://www.sonarqube.org/sonarqube-7-9-lts/

---

> [SonarQube](https://www.sonarqube.org/) (formerly Sonar) is an open-source platform developed by
> SonarSource for continuous inspection of code quality to perform automatic reviews with static
> analysis of code to detect bugs and code smells on many programming languages.

SonarQube follows [Semantic Versioning](https://semver.org/). A new major or minor version is
released every 2 months, and a new LTS release is declared approximately every 18 months.

Only the latest major release receives active support (updates and patches). During that time, the
previous major release receives LTS support (security patches and fixes of blocker bugs) until the
next LTS is declared. This support policy is the same for the Community, Developer, Enterprise and
Data Center editions.

Release notes for all version can be found on [What's New in SonarQube](https://www.sonarqube.org/whats-new/).
