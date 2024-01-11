node
{
    
     def branchName = env.BRANCH_NAME 
     def workspace="C:\\Clearing_Workspace"+branchName
    stage("Clearing Workspace")
    {
       
         if(branchName=="develop"||branchName=="main"||branchName=="Clearworkspace"||branchName=="function1"||branchName=="Release")
         {
            echo "no Need to delete"
         }
         else 
         { 
            dir(workspace)
            {
               

               bat 'rmdir /q /s .'
           }
           
         }



    }
}
