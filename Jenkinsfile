node('worker_node') {
    
        stage('source') {
	        
		     git 'https://github.com/ankurmishra727/JenkinsWithJenkinsFile2.git'




		     	}



			      stage('deploy') {
			                
			     sh 'python test.py'
				      
				      
				      
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
