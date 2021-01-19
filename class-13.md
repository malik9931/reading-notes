## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS


<p>Historically, web applications have had none of these luxuries. Cookies were invented early in the web&#8217;s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

<ul>
<li>Cookies are included with every <abbr>HTTP</abbr> request, thereby slowing down your web application by needlessly transmitting the same data over and over
<li>Cookies are included with every <abbr>HTTP</abbr> request, thereby sending data unencrypted over the internet (unless your entire web application is served over <abbr>SSL</abbr>)
<li>Cookies are limited to about 4 KB of data &mdash; enough to slow down your application (see above), but not enough to be terribly useful
</ul>

<p>What we really want is

<ul>
<li>a lot of storage space
<li>on the client
<li>that persists beyond a page refresh
<li>and isn&#8217;t transmitted to the server
</ul>

![nasl](https://lh3.googleusercontent.com/proxy/S40JgeQSsH5_dAlYVw5TLbKuUzXPxJa3WlPGJkas3Mn1U2hy9wff8HLH52fWN3a4TIkyt_gIWNMiXBNp_B2XdpleW9xTlvvuZSGafies6ozJL9G4ad60UbHohRc69zC6JiDRMwRitTn5ck6FzdfdsmPicRFeVaZuRDKN32OeE7dBFfbr3Bf1oU6gVOnnRyXVWYa57YCzBcZUEFCz-WiykapkJZ1Tckhy)


![sd](https://www.researchgate.net/profile/Azzam_Sleit/publication/320614525/figure/fig1/AS:553282116767744@1508924144633/Modern-Web-Application-Architecture-and-Running-Environments-20.png)

<table class=st>
<caption>StorageEvent Object</caption>
<thead>
<tr class=ho><th>Property<th>Type<th>Description
<tbody>
<tr class=zebra><th><code>key</code><td>string<td>the named key that was added, removed, or modified
<tr><th><code>oldValue</code><td>any<td>the previous value (now overwritten), or <code>null</code> if a new item was added
<tr class=zebra><th><code>newValue</code><td>any<td>the new value, or <code>null</code> if an item was removed
<tr><th><code>url</code><sup>*</sup><td>string<td>the page which called a method that triggered this change
<tfoot>
<tr><td colspan=3>* Note: the <code>url</code> property was originally called <code>uri</code>. Some browsers shipped with that property before the specification changed. For maximum compatibility, you should check whether the <code>url</code> property exists, and if not, check for the <code>uri</code> property instead.
</table>
