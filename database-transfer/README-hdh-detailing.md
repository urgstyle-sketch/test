# Encrypted database transfer

`hdh-detailing-hb-encrypted.7z` is an AES-256 encrypted archive with encrypted headers. The password is provided separately in the private conversation and is not stored in this repository.

1. Download the `.7z` file and extract it with 7-Zip using the password provided privately.
2. The extracted `hdh-detailing-hb.sql.zip` is ready for phpMyAdmin.
3. In phpMyAdmin, select a NEW EMPTY destination database and import the inner ZIP. It contains DROP TABLE statements for the existing WordPress table names.
4. Set the new database connection details in the site's wp-config.php. The table prefix is `wp_`.

The database was prepared and test-imported before encryption. Website files must be cleaned separately before release.

Encrypted archive SHA-256:

`468d95274236e8668db0ee1e3e01e6fae2d2357bbc235c810782d8f33379227c`
