pipeline{
  agent any
    stages{
      stage(clone){
        steps{
        git clone "https://github.com/Keerthi26099/kko.git"
    }
      }
      stage(build)
      {
        steps{
        javac K.java
      }
      }
      stage(run)
      {
        steps{
          
        java K.java
      }
      }
  }
}
