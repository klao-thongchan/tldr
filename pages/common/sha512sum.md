# sha512sum

> Calculate SHA512 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

- Calculate the SHA512 checksum for one or more files:

`sha512sum {{path/to/file1 path/to/file2 ...}}`

- Calculate and save the list of SHA512 checksums to a file:

`sha512sum {{path/to/file1 path/to/file2 ...}} > {{path/to/file.sha512}}`

- Calculate a SHA512 checksum from `stdin`:

`{{command}} | sha512sum`

- Read a file of SHA512 checksums and filenames and verify all files have matching checksums:

`sha512sum {{[-c|--check]}} {{path/to/file.sha512}}`

- Only show a message for missing files or when verification fails:

`sha512sum {{[-c|--check]}} --quiet {{path/to/file.sha512}}`

- Only show a message when verification fails, ignoring missing files:

`sha512sum --ignore-missing {{[-c|--check]}} --quiet {{path/to/file.sha512}}`

- Check a known SHA512 checksum of a file:

`echo {{known_sha512_checksum_of_the_file}} {{path/to/file}} | sha512sum {{[-c|--check]}}`
