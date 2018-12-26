## Script Cek mutasi BNI

Hasil waktu luang pas weekend.

Cara pakai. 

		require_once 'src/CekBNI.php';
		$config = [
		        'credential' => [
		            'username' => 'jenengmu',
		            'password' => 'passwordmu'
		        ],
		        'nomor_rekening' => '0400xxxxxx', //No. Rekening
		        'range' => [
		            'tgl_akhir' => date('d-M-Y',strtotime('2018-07-31')),
		            'tgl_awal' => date('d-M-Y',strtotime('2018-07-01'))
		        ],
		];
		
		$bni = new CekBNI($config);
		var_dump($bni->toArray());

lebih lengkap lihat example.php

[Butuh bantuan lain? hubungi saya via telegram](https://t.me/galihazizif)