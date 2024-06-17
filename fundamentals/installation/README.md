# 📝 Installation

Download the script from the repository, execute it and let Snowball take care of you.

```sh
curl -fsSL https://snowball-lang.github.io/install/script.sh | bash -s -- -y
```

**note:** Even though we use `sudo`, it's possible to not use sudo but it's not recommended. If using sudo, you must use **`-E`** as arg to get the user env variables.

We also make use of the `-y` parameter that tells the install script to avoid all prompts and take the recomended paths

<details>

<summary>Adding snowball to $PATH</summary>

The snowball installer will do this automatically but just in case, you can execute:

```sh
export PATH="$PATH:~/.snowball/bin"
```

</details>

{% content-ref url="common-install-issues.md" %}
[common-install-issues.md](common-install-issues.md)
{% endcontent-ref %}
