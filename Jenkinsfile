node
{
    
     def branchName = env.BRANCH_NAME 
     def workspace="C:\\Clearing_Workspace"+branchName
    stage("Clearing Workspace")
    {
       
         def branchesToExclude = ["develop", "main", "Clearworkspace", "function1", "Release"]

            if (branchesToExclude.contains(branchName)) {
                echo "No need to delete the workspace"
            } else {
                dir(workspace) {
                    deleteDir()
                }
            }



    }
}
