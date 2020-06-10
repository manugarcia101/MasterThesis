<h2># MasterThesis</h2>

<p>Master thesis Exodus project aims to replicate <a href="https://www.numbeo.com/">Numbeo website</a> with a modern interface,
a new concept of Quality of life, based in the local marks of every of the subindexes that compound it, rather than a comparison
with a model mark city as in case of Numbeo.</p>

<h4>To run the app in your own host, you need the following requirements:</h4>
<p>Apache server + mysql database installed(I personally recommend xampp server)</p>
<p>Composer and PHP v7.2+ installed</p>
<p>Python v3.7.x+</p>

<h4>Deploy:</h4>
<p>Run Laravel backend with "php artisan serve" command and check that it works</p>
<p>Create an empty database in localhost/phpmyadmin/ (To run xampp server you will need to do: sudo /opt/lampp/lampp start, and stop other posible server running on ports 80, 443 and 3306)<p>
<p>Run Laravel migrations "php artisan migrate" command and check that it works (Change the connection params in .env file to connect to your new database)</p>
<p>Check that the new Databases have been created</p>
<p>In the database folder, search for populatedb.py and run it python (Change the connection params to connect to your new database)</p>
<p>Check in phpmyadmin that the database has been populated</p>
<p>Run again "php artisan serve".</p>
<p>Copy the frontend /dist folder to your /htdocs folder (in xampp).</p>
<p>Open localhost/dist/application/ and check that it works.</p>
