node {
    git 'git@github.com:Demengjkee/vault_repo_1.git'
    sh 'ls -la; ls -la cih/'
    def test = load("cih/Test.groovy")
    println(test)
    def str = test("str");
    sh '${str}'
/*
  def vaultIp = "34.250.137.247"
  def vaultAddr = "http://${vaultIp}:8200"
  withCredentials([string(credentialsId: 'GITHUB_TOKEN', variable: 'TOKEN')]) {
     sh """
       docker run -v ${WORKSPACE}:/mnt --rm --cap-add=IPC_LOCK -e "VAULT_ADDR=${vaultAddr}" vault /bin/sh -c "
       vault auth -method=github token=${TOKEN};
       vault read secret/epam/password;
       vault read secret/sp5/password;"              
     """
  }
*/
}
