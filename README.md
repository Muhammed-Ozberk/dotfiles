# Dotfiles

Bu proje, terminal ayarlarınızı kişiselleştirmenize yardımcı olmak için kullanılan bir konfigürasyon deposudur. Bu repo, Zsh terminali ve Powerlevel10k temasının özelleştirilmiş ayarlarını içerir.

## Terminal Görüntüsü

Aşağıdaki terminal ekran görüntüsü, bu konfigürasyon dosyaları ile elde edilecek görünümü göstermektedir:

![Terminal Screenshot](zsh-example.png)

## Kurulum

Aşağıdaki adımları takip ederek terminalinizde bu görünümü elde edebilirsiniz.

### **1. Gerekli Araçların Yüklenmesi**

İlk olarak, Zsh ve Powerlevel10k'yi yüklemeniz gerekmektedir. İşletim sisteminize uygun talimatları aşağıda bulabilirsiniz.

#### **Linux ve macOS**

1. **Zsh Kurulumu**

   Zsh genellikle Linux ve macOS sistemlerinde varsayılan olarak bulunur. Eğer yüklenmemişse, aşağıdaki komutlarla yükleyebilirsiniz:

   - **Ubuntu/Debian:**

     ```bash
     sudo apt update
     sudo apt install zsh
     ```

   - **Fedora:**

     ```bash
     sudo dnf install zsh
     ```

   - **macOS (Homebrew ile):**

     ```bash
     brew install zsh
     ```

2. **Powerlevel10k Teması Kurulumu**

   Powerlevel10k temasını yüklemek için önce [Oh My Zsh](https://ohmyz.sh/) kurulumunu yapmanız gerekebilir. Daha sonra Powerlevel10k'yi yükleyebilirsiniz:

   ```bash
   # Oh My Zsh'i kurun (eğer daha önce kurulu değilse)
   sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

   # Powerlevel10k'yi yükleyin
   git clone --depth=1 https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
   ```

#### **Windows**

Windows üzerinde Zsh ve Powerlevel10k kullanmak için [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/) veya [Cygwin](https://www.cygwin.com/) kullanabilirsiniz.

1. **WSL veya Cygwin Kurulumu**

   WSL veya Cygwin'i yükledikten sonra, yukarıdaki Linux ve macOS talimatlarını takip ederek Zsh ve Powerlevel10k'yi kurabilirsiniz.

### **2. Depoyu Klonlayın**

Bu repo dizinini yerel bilgisayarınıza klonlayarak gerekli konfigürasyon dosyalarını elde edebilirsiniz:

```bash
git clone <your-git-repo-url> ~/dotfiles
```

### **3. Dosyaları Yükleyin**

Klonlanan dosyaları terminal konfigürasyonunuz için uygun konumlarına taşıyın:

```bash
cp ~/dotfiles/.zshrc ~/.zshrc
cp ~/dotfiles/.p10k.zsh ~/.p10k.zsh
```

### **4. Zsh'yi Yeniden Başlatın**

Yapılandırma değişikliklerinin etkili olabilmesi için Zsh oturumunu yeniden başlatmanız gerekmektedir:

```bash
exec zsh
```

## Notlar

- `~/.zshrc` dosyası, Zsh terminalinizin genel ayarlarını ve eklentilerini içerir.
- `~/.p10k.zsh` dosyası, Powerlevel10k temasının özelleştirilmiş ayarlarını içerir.
- Bu dosyalar, terminal deneyiminizi kişiselleştirmenize yardımcı olur.

## Lisans

Bu projede kullanılan dosyalar kişisel kullanım içindir. Başka bir şekilde dağıtım yapmadan önce lisans şartlarını gözden geçirdiğinizden emin olun.