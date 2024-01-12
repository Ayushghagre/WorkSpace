node {
    properties([
        pipelineTriggers([
            cron('*/5 4-23 * * 1-5')

        ])
    ])

    def branchName = env.BRANCH_NAME
    def workspace = "C:\\Clearing_Workspace\\" + branchName

    try {
        stage("Clearing Workspace") {

def branchesToExclude = ["develop", "main", "Clearworkspace", "function1", "Release"]

            if (branchesToExclude.contains(branchName)) {
                echo "No need to delete the workspace"
            } else {
                dir(workspace) {
                    deleteDir()
                }
            }
        }
    } catch (Exception e) 
    {
        echo "Encountered an exception"
        echo e.toString()
    }
}
