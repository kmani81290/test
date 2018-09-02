node(){
    stage 'Checkout'
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'kamrajshahapure', url: 'https://github.com/kamrajshahapure/Test']]])
	
	stage 'Build'
	bat 'ant clean compile jar'
	stage 'Echo'
	echo 'my first pipeline'
}
