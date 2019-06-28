node('ansible')
{
    stage('deploy')
    {
        dir('/home/appserver/srini/jenkins/workspace')
        {
          ansiblePlaybook(
          playbook: 'deployface-UI.yml',
         //This is the file name we have created in ansible
          inventory: 'inventory',
          installation: 'ansible2.4.2.0',
          extras: "-e 'version=${version}'"
          )
        }
    }
}
