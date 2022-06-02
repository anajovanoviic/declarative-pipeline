pipeline {
agent any
stages {
stage("Stage 1"){
steps {
script {
echo "Hello ${params.name}"
if (params.office) {
echo "Hey ${params.name} have fun at the office!"
} else {
echo "Why are you not in the office ${params.name} ?"
}
echo "${params.name} you are ${params.age} years old."
}
}
}
}
}
