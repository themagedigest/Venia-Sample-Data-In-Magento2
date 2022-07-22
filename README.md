# Venia-Sample-Data-In-Magento2

Steps to follow - 

1. composer config --no-interaction --ansi repositories.venia-sample-data composer https://repo.magento.com
2. composer require --no-interaction --ansi magento/venia-sample-data:*
3. bin/magento setup:upgrade
4. bin/magento indexer:reindex
5. bin/magento catalog:images:resize
6. php bin/magento setup:static-content:deploy -f
7. chmod -R 777 var/ pub/ vendor/ generated/ app/
