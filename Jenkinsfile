node{
checkout scm;
stage('load'){
file=load "sonar.properties"
echo "${file}"
def lines=file.split("\n");
def len=lines.length;
echo "${len}"
def paramString = "";
    for(int i=0;i<len;i++)
    {
        paramString = paramString + " "+ "-D"+"${lines[i].trim()}";
    }
echo "${paramString}"
}
}
