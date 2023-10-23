# hello

This is a hello world demo Java (Maven) package.

## Prerequisites

### Group ID in OSSRH

1. [Create a new Sonatype JIRA account](https://issues.sonatype.org/secure/Signup!default.jspa), if you don't have one yet.
2. [Create a new JIRA issue for OSSRH](https://issues.sonatype.org/secure/CreateIssue.jspa?issuetype=21&pid=10134) as follows:

   - **Summary**: Something like `Create new com.yourdomain project`
   - **Description**: Something like `Create new groupId for my open source project`
   - **Group Id**: Your group Id e.g. `com.yourdomain`
   - **Project URL**: Your website or your GitHub repository e.g. `https://github.com/pacroy/hello-package`
   - **SCM URL**: Your Git repository URL e.g. `https://github.com/pacroy/hello-package.git`
   - **Username**: Your JIRA username

    Note: See my issue [OSSRH-96002](https://issues.sonatype.org/projects/OSSRH/issues/OSSRH-96002) as an example.

3. Wait until the *Bot Central-OSSRH* comment with instruction to add a DNS `TXT`` record (In my case, it took 8 minutes).
4. Add DNS `TXT` record per instruction and set ticket status to `Open`.
5. Wait until the *Bot Central-OSSRH* prepare your new group ID and comment with instruction on how to publish (In my case, it took ~30 minutes).

### GPG Key

1. Generate a new GPG key using command `gpg --full-generate-key` and choose the following options:

   - **Kind of key**: `(1) RSA and RSA`
   - **Key size**: `4096`
   - **Validity period**: For example `1y`
   - **Real name**: Input your first name and last name
   - **Email address**: Your email addess or use GitHub one e.g. `username@users.noreply.github.com`
   - **Comment**: Label your key in case you have many key so you can remember the purpose of each one e.g. `username@hostname`.

    Choose (O)kay and enter a passphrase to protect your key.

2. aaa



## Build & Publish

1. aaa

## Install

```sh

```

## Usage

```java

```

## References

- [How to Publish a Java Library to Maven Central | Sergio Martin Rubio](https://sergiomartinrubio.com/articles/how-to-publish-a-java-library-to-maven-central/)
- [Maciej Walkowiak | How to publish a Java library to Maven Central - Complete Guide](https://maciejwalkowiak.com/blog/publish-java-library-maven-central/)
- [Publish Java Packages to Maven Central Repository | DevDungeon](https://www.devdungeon.com/content/publish-java-packages-maven-central-repository)
- [Beginner guide to Maven Central publishing - DEV Community](https://dev.to/julbrs/beginner-guide-to-maven-central-publishing-3jio)
- [Apache Maven - The Central Repository Documentation](https://central.sonatype.org/publish/publish-maven/#deployment)