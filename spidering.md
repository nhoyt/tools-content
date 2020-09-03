[FAE](/tools/fae) is a web application that evaluates the pages in a website by using a technique known as web spidering. The main parameters needed for spidering, and hence evaluation, are:

* starting URL
* depth level (explained by example below)
* domain and path constraints for following links

### Domain and path constraints

When you start an evaluation in FAE, you specify domain and path constraints that control which pages the spidering algorithm will analyze. For a multi-page evaluation, these are found under the ‘Follow Links In’ heading. The choices are:

* ‘Specified domain only’ (default): Use the domain of the starting URL and follow any link within that domain.
* ‘With specified path’ (checkbox): When the starting URL includes path information, only follow links within the specified domain that have the same path.
* ‘Specified domain and all of its next-level subdomains’: For example, if *www.mydomain.com* was specified as the starting URL, also follow links in other subdomains, such as *abc.mydomain.com*.

### Example of FAE website evaluation using web spidering

Taking the depth level as 3, here is an example of how the algorithm works:

1. The top-level page, specified as the starting URL, is evaluated and its results are saved.
1. For each link found on the top-level page that satisfies the domain and path constraints, access the linked second-level page, evaluate it and save its results.
1. For each link found on a second-level page that satisfies the domain and path constraints, access the linked third-level page, evaluate it and save its results.
1. Once FAE has evaluated the top-level page and all second- and third-level pages with URLs that satisfy the specified domain and path constraints, spidering stops since the depth level is 3.
1. Process all of the page-level results that were saved and aggregate these results into a summary report for the entire website.
