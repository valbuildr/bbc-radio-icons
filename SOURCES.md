On the BBC Sounds website, you can view all BBC Radio stations. ([here](https://www.bbc.co.uk/sounds/stations))

Right-clicking on one of the network icons you can find an SVG, which should have a src property of something like this: `https://sounds.files.bbci.co.uk/3.7.0/networks/bbc_sounds_news/colour_default.svg`

Opening this link will let you view the raw SVG, which you can save by right-clicking and clicking 'Save as'.

But if you want the wordmark, you'll have to change the `colour_default.svg` to something else.

- For a white wordmark, replace it with `blocks-white_default.svg`
- For a coloured wordmark, replace it with `blocks-colour_default.svg`

For local radio networks, you can simply get the station's ID by clicking on the station name and looking at the end of the URL.

- For BBC Radio Cambridgeshire, this is `bbc_radio_cambridge`.
- For BBC Radio London, this is `bbc_london`.

You can then take that ID and put it into the link using this formula: `https://sounds.files.bbci.co.uk/3.7.0/networks/{network id}/{file}`.

- For BBC Radio Cambridgeshire's icon, the link would be `https://sounds.files.bbci.co.uk/3.7.0/networks/bbc_radio_cambridge/colour_default.svg`.
- For BBC Radio London's coloured wordmark, the link would be `https://sounds.files.bbci.co.uk/3.7.0/networks/bbc_london/blocks-colour_default.svg`.
- For BBC Radio Kent's coloured wordmark, the link would be `https://sounds.files.bbci.co.uk/3.7.0/networks/bbc_radio_kent/blocks-white_default.svg`.

Do note that from my testing, there's one local network, Radio Solent Dorset, that doesn't work with this, and you'll have to replace `networks` with `services`.
