GitHub Workflow Deployment
=========================================================
In [Deployment Setup](#deployment-setup) we defined the deployment branch in the `.github/workflows/deploy.yml` [file][deploy], which is used then used for the deployment, whenever performing `git push`. You are free to use any branch, other than the `gh-pages`, keeping in mind that only upon the `git push`, the workflow will be triggered.

The workflow deployment itself is tracked by the status indicator in the repository, in this case a beige-brown dot <strong><b><font color='peru'>⏺</font></strong></b>, which if clicked on, will show the running status, and the deployment details. As mentioned, the deployment takes approx. 2 minutes to finish.

<center>
<figure>
    <!-- <a href='https://github.com/open-energy-transition/data-science-for-esm/settings/pages'> -->
    <img src='https://raw.githubusercontent.com/open-energy-transition/data-science-for-esm/stanford/data-science-for-esm/_images/05_deployment_status.png' width='85%'style='vertical-align:middle;border:5px solid paleturquoise;margin:30px 30px' />
    <!-- </a> -->
    <figcaption>Deployment status upon <code>git push</code> to the branch specified in the <em>deploy.yml</em> file</figcaption>
</figure>
</center>

Upon a successful deployment, indicated by the deploy status:
* successful: a green thick <strong><b><font color='green'>🗸</font></strong></b>
* unsuccessful: a red cross mark <font color="red">🗶</font>,
you should be able to see the changes taking place in the specified `github.io` URL.

<center>
<figure>
    <!-- <a href='https://github.com/open-energy-transition/data-science-for-esm/settings/pages'> -->
    <img src='https://raw.githubusercontent.com/open-energy-transition/data-science-for-esm/stanford/data-science-for-esm/_images/06_successful_deployment.png' width='85%'style='vertical-align:middle;border:5px solid paleturquoise;margin:30px 30px' />
    <!-- </a> -->
    <figcaption>Successful deployment, after a finalized <code>jupyter book build</code> run</figcaption>
</figure>
</center>