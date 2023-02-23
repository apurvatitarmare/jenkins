pipeline {

agent any
stages{

stage ("stage-1")   {
steps {
sh "git clone https://github.com/apurvatitarmare/jenkins.git"

}
}

stage ("stage-2")   {
steps  {
sh "cp -r /root/.jenkins/workspace/as-6/jenkins/index.html /var/www/html"
}

}

stage ("stage-3")   {
steps  {
sh "service httpd restart:cd /var/www/html:chmod 777 index.html"
}

}


}



}
