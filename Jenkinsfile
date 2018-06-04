node('worker_node') {
    
        stage('source') {
	        
		     git 'https://github.com/ankurmishra727/JenkinsWithJenkinsFile2.git'




		     	}



			      stage('deploy') {
			                
					         sh 'python test.py'
				      
				      
				      def choice = input message: '<message>', 
                                      parameters: [choice(choices: "choice1\nchoice2\nchoice3\nchoice4\n",
                                      description: 'Choose an option', name: 'Options')]
				      
				      
				      
				                 properties([
  pipelineTriggers([
    upstream(
      threshold: hudson.model.Result.SUCCESS,
      upstreamProjects: 'Git_Simple_1'
    )
  ])
])
						 	 


							 	  }




								      }
