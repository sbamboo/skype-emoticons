# Skype Emoticons
A repository with the goal to collect the skype emoticons in a fetchable way using indexing.

## The repository
The repository will contain multiple collections if more variants or updates are found/created.<br>
Currently it contains `ms-gif-wbg` (*"Microsoft .GIF With Background"*) which is the assets avaliable at [support.microsoft.com/en-us/skype/what-is-the-full-list-of-emoticons](https://support.microsoft.com/en-us/skype/what-is-the-full-list-of-emoticons-01af0c65-529f-4a4d-8e3a-a393033a359a)

## The collections
Inside each collection is the assets themselves under the `emoticons` folder aswell as a json-index (`emoticons.index.json`) and markdown overview (`emoticons.index.md`). 
Some collections might also include an alternative index with original links these are prefixed so `{prefix}.emoticons.index.json`.
Incase licensing is avaliable a `LICENSE.txt` file may be found in the collection folder.

## Json Index
The json index follows the following format:
```JSONC
{
    "{category}": {
        "{emoticon_id}": {
            "name": "{emoticon_name}",
            "shortcuts": [
                "{emoticon_shortcut}", // Example `(laugh)`
                ...
            ],
            "textmojis": [
                "{emoticon_textmoji}", // Example `:D`
                ...
            ],
            "url": "{emoticon_url}"
        },
        ...
    },
    ...
}
```