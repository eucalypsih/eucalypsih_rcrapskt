# eucalypsih_rcrapskt

```
owner="eucalypsih";repo="eucalypsih_rcrapskt";git clone -q --filter=blob:none --sparse git@github.com:${owner}/${repo}.git && sleep 0.5 && cd $repo && sleep 0.5 && un="eucalypsih";ue="eucalypsih@gmail.com";git checkout main && sleep 0.5 && git config user.name "$un" && sleep 0.5 && git config user.email "$ue" && sleep 0.5 && git config gpg.format ssh && sleep 0.5 && git config user.signingkey ~/.ssh/id_rsa.pub && sleep 0.5 && git config commit.gpgsign true && sleep 0.5 && git config gpg.ssh.allowedSignersFile ~/.ssh/allowed_signers
```
`owner="eucalypsih";repo="eucalypsih_rcrapskt";git clone -q --filter=blob:none --sparse git@github.com:${owner}/${repo}.git && sleep 0.5 && cd $repo && sleep 0.5 && un="eucalypsih";ue="eucalypsih@gmail.com";git checkout main && sleep 0.5 && git config user.name "$un" && sleep 0.5 && git config user.email "$ue" && sleep 0.5 && git config gpg.format ssh && sleep 0.5 && git config user.signingkey ~/.ssh/id_rsa.pub && sleep 0.5 && git config commit.gpgsign true && sleep 0.5 && git config gpg.ssh.allowedSignersFile ~/.ssh/allowed_signers`


```
git sparse-checkout list
```

```
git sparse-checkout add frasa_kt
```

```
micro .git/info/sparse-checkout
```

```
git sparse-checkout reapply
```



```
kotlinc hello.kt -include-runtime -d hello.jar -J-Djansi.skip=true 2>/dev/null
```

```
java -jar hello.jar
```

```
echo "alias kotlinc='kotlinc 2>/dev/null'" >> ~/.bashrc
```

```
fun main() {
    println("Halo dari Kotlin di Termux!")
}

```



Opsi A: Jika menggunakan `app/build.gradle` (Format Groovy - Umum)
Buka file `app/build.gradle` menggunakan editor teks (seperti `nano app/build.gradle`), lalu tambahkan baris konfigurasi berikut di bagian paling bawah file:
```
tasks.named('run') {
    standardInput = System.in
}

```

Opsi B: Jika menggunakan `app/build.gradle.kts` (Format Kotlin DSL)
Jika file konfigurasi Anda berakhiran `.kts`, buka filenya (`nano app/build.gradle.kts`) dan tambahkan baris berikut di bagian paling bawah:
```
tasks.named<JavaExec>("run") {
    standardInput = System.`in`
}

```
