# Personal Maven Repo

*Personal maven repo for projects that aren't primarily used by others.  If you see something you'd like to use in this repo, let me know and we should talk about putting it in Maven Central.*

### Add

    $ mvn deploy -DaltDeploymentRepository=repo::default::file://$HOME/Development/repo

### Use

#### Maven

    <repositories>
        <repository>
            <id>com.github.ryanbrainard.repo</id>
            <url>https://raw.github.com/ryanbrainard/repo/master</url>
        </repository>
    </repositories>

#### SBT

    resolvers ++= Seq("com.github.ryanbrainard.repo" at "https://raw.github.com/ryanbrainard/repo/master")
