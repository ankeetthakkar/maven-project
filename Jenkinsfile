pipeline
{

 agent any
 {

stage "scm checkout"
git 'https://github.com/ankeetthakkar/maven-project.git'

}

stage "code test"
withMaven(maven: 'Local Maven') {
    sh 'mvn test'
}
}

}
}
