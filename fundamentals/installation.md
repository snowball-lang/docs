# 📝 Installation

<details>

<summary>Downloading and executing script</summary>

Download the script from the repository, execute it and let Snowball take care of you.

```sh
curl -fsSL https://raw.githubusercontent.com/snowball-lang/snowball/dev/scripts/install.sh | sudo -E bash -s -- -y
```

**note:** Even though we use `sudo`, it's possible to not use sudo but it's not recommended. If using sudo, you must use **`-E`** as arg to get the user env variables.

</details>

<details>

<summary>Adding snowball to $PATH</summary>

The snowball installer will do this automatically but just in case, you can execute:

```sh
export PATH="$PATH:~/.snowball/bin"
```

</details>
