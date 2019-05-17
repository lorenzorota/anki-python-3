# anki-python-3

Collaboration on Anki flashcards for mastering python3 programming concepts, semantics and syntax

## Getting Started

Make sure to have 

### Prerequisites

* Anki (latest version)
* CrowdAnki (add-on)


### Installing

Make sure to have the latest version of Anki-desktop installed. This can be obtained from [here](https://apps.ankiweb.net/)

Once you have it installed, proceed to download the CrowdAnki add-on, by either following the instructions on [https://ankiweb.net/shared/info/1788670778](https://ankiweb.net/shared/info/1788670778), or simply going to the Anki-desktop menu item ``` Tools > Add-ons > Get Add-ons...``` and entering the code ``` 1788670778 ```


### Configuring CrowdAnki

To configure CrowdAnki, open the menu item ``` Tools > Add-ons ``` and highlight the CrowdAnki add-on. Then press ``` Config ``` to open up the JSON formatted configuration.

Here is a sample configuration:

```
{
    "automated_snapshot": false,
    "snapshot_path": "~/Anki",
    "snapshot_root_decks": []
}
```

Ensure to have the ``` snapshot_path ``` line configured correctly, as it will enable you to automatically commit changes to all your Decks stored in the ``` ~/Anki/<username> ``` folder, by running the ``` File > CrowdAnki: Snapshot ``` menu item. 

### Contributing to (this) repository

To contribute to this repository, make sure to be in the ``` ~/Anki/<username> ``` folder and simply run the following command from your terminal:

```
git clone https://github.com/lorenzorota/anki-python-3.git python-3
```

From Anki-desktop, go to ``` File > CrowdAnki: Import from disk ```, and select the folder that you just retrieved.
Running ``` File > CrowdAnki: Snapshot ``` will automatically commit changes to this repository. You will then only need to run:

```
git push
```

A manual approach would be to navigate to your deck (in this case ``` python-3 ```), hovering over the configuration icon and pressing Export. Select the ``` Export format: CrowdAnki Json representation (\*directory) ```, press ``` Export... ```, and save to the ``` ~/Anki/<username> ``` folder. Then run the following commands

```
git pull
git add .
git commit -a -m "Message to indicate changes made"
git push
```

That's really all there is to it

## Authors

* **Lorenzo Rota** - *Setting up the repository* - [lorenzorota](https://github.com/lorenzorota)
* **Paul Côté** - *Co-authoring the Anki Deck* - [paulccote](https://github.com/paulccote)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the GPL-3.0 License - see the [LICENSE.md](LICENSE.md) file for details
