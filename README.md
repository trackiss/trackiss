## trackiss

```scala
case class MyProfile extends GitHubProfile (
    name      = "trackiss".aka("とらきす")
    locate    = Japan.Gifu,
    birthDate = LocalDate.parse("2000-11-24"),

    history = History.empty[Job]
      .join("岐阜工業高等専門学校 電気情報工学科")
      .drop("岐阜工業高等専門学校 電気情報工学科")
      .join("名古屋工学院専門学校 高度情報学科")
      .graduate("名古屋工学院専門学校 高度情報学科")
      .join("Chatwork株式会社")
      .asScala,

    links = Map(
        "GitHub"      -> this.toUrl,
        "X"           -> "https://x.com/twi_trackiss",
        "HatenaBlog"  -> "https://trackiss.hateblo.jp",
        "Qiita"       -> "https://qiita.com/trackiss",
        "SpeakerDeck" -> "https://speakerdeck.com/trackiss"
    )
)
```
