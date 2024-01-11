node
{
    
     def branchName = env.BRANCH_NAME 
     def workspace="C:\\Clearing_Workspace"+branchName
    stage("Clearing Workspace")
    {
       
         if(branchName=="develop"||branchName=="main"||branchName=="Clear_workspace"||branchName=="function1"||branchName=="Release"||branchName=="patch")
         {
            echo "no Need to delete"
         }
         else 
         { 
            dir(workspace)
            {
               

               deleteDir();
           }
           
         }



    }
}
