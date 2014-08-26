nibse-php
=========

Register for your Access Token at https://www.wmcex.com/gettoken


<h1>Simple Usage</h1>

include_once 'nibse.php';
$nibse = new nibse(YOUR_ACCESS_TOKEN);

#optional $WALLET_LABEL is a public name for this wallet
if ($nibse->CreateWallet([$WALLET_LABEL]))
{
  $wallet_address = $nibse->walletAddress;
  $wallet_key = $nibse->walletKey;
}
