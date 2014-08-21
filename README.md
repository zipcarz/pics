pics
====
		 import (
 	"encoding/json"
 	"fmt"
+	"os"
 	. "github.com/openshift/geard/cmd"
 	"github.com/openshift/geard/router"
 	rjobs "github.com/openshift/geard/router/jobs"
 	"github.com/openshift/geard/transport"
 	"github.com/spf13/cobra"
-	"os"
 )
 
 type Command struct {
@@ -46,7 +46,7 @@ func (e *Command) RegisterRouterCmds(parent *cobra.Command) {
 
 	testCmd = &cobra.Command{
 		Use:   "delete-frontend",
-		Short: "Delete an existing from the router.",
+		Short: "Delete an existing frontend from the router.",
 		Run:   e.removeFrontend,
 	}
 	routerCmd.AddCommand(testCmd)

