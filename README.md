# sonarqube-scripts
A couple of useful scripts for SonarQube

replay-the-past.sh
Replays the past of a full git repository

usage: replay-the-past.sh [-g <git-repo>] [-s <scan command>]
-g: .git URL corresponding to the repo to replay. If not provided, script assumes that you are already in a git root directory of that repo
-s: Commadn to run to scan. If not provide assumes mvn clean org.jacoco:jacoco-maven-plugin:prepare-agent install -Dmaven.test.failure.ignore=true sonar:sonar

