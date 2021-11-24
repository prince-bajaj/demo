pipeline{
		agent {
		    label 'Slave-Node'
		    
		}
		stages{
				stage('build'){
								steps{
										echo "building ist stage!!"
								}
				}
				stage('Test'){
								steps{
										echo "testing stage!!"
								}
				}
				stage('Deploy'){
								 steps{
										 echo "deploy product!!"
			
								 }
				}
		}
		
		
		post{
			always{
					echo "this will run always!!"
			      }
			success{
					echo "this will run when only success!!"
				   }
			failure{
				    echo "this will run when failure occurs!!"
				   }
			unstable{
					 echo "this will occur when there is unstable result!!"
				    }
			changed{
				     echo "this will occur only if state changed.!!"
					 echo  "for example if pipeline was failing and now its passing!!"
				   }
		}


}
