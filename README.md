nibse-php
=========

Register for your Access Token at https://www.wmcex.com/gettoken

#Simple Usage

include_once 'nibse.php';<br>
$nibse = new nibse(YOUR_ACCESS_TOKEN);<br>

<!--optional $WALLET_LABEL is a public name for this wallet-->
if ($nibse->CreateWallet([$WALLET_LABEL]))<br>
{<br>
  $wallet_address = $nibse->walletAddress;<br>
  $wallet_key = $nibse->walletKey;<br>
}
