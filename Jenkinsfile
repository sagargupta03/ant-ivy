pipeline
{
	agent any
	stages
	{
		stage('Build') 
		{
		steps {
                  def antVersion = 'Ant1.10.5'
                   withEnv( ["ANT_HOME=${tool antVersion}"] ) {
                  sh '$ANT_HOME/bin/ant target1 target2'
                       }

               	echo 'Building..'			
		      }
		}
		stage('Test')
		{
		steps {
		echo 'Testing..'
		      }
		}
		stage('Deploy')
		{
                
                steps {
		echo 'Deploying....'
		      }
		}
	}
}
