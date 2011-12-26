<h1>How?</h1>
<p>To use, go to <i>/Library/Application Suppport/Titanium/mobilesdk/osx//iphone/Classes/</i> and paste the files of this GitHub directory. <b>Don't forget to make a backup of your files</b></p>
<h1>Coding</h1>
<p>To make animations, you can create a SearchBar with the cancel button hide. When focus you show de cancel button and when blur the searchBar, you hide the cancel button. See this example:</p>
<pre>var searchBarForExample = Ti.UI.createSearchBar({
    hintText:"Treinamentos.mobi",
    showCancel:false
});

searchBarForExample.addEventListener("focus", function() {
    searchBarForExample.showCancel = true;
});

searchBarForExample.addEventListener("blur", function() {
    searchBarForExample.showCancel = false;
});</pre>