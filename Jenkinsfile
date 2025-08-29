@Library('jenkins-shared-library') _

def configMap = [
    project : "roboshop",
    component : "payment"
]

if ( ! env.BRANCH_NAME.equalsIgnoreCase('main') ) {   // ig not equals to main branch
    pythonEKSPipeline(configMap)    // by default it will call, call function inside this pipeline
}
else {
    echo "Please proceed with PROD process"
}
