## trackiss

```scala
case class MyProfile(
    name      = "Ryuki Kobayashi" aka "trackiss",
    location  = Japan.Gifu,
    birthDate = LocalDate.parse("2000-11-24"),

    history = History.empty[Job]
      .join("岐阜工業高等専門学校 電気情報工学科")
      .drop("岐阜工業高等専門学校 電気情報工学科")
      .join("名古屋工学院専門学校 高度情報学科")
      .graduate("名古屋工学院専門学校 高度情報学科")
      .join("Chatwork株式会社").asScala
      .renameTo("Chatwork株式会社" -> "株式会社kubell"),

    links = Map(
      "GitHub" -> this.url,
      "X"      -> "https://x.com/twi_trackiss",
      "Blog"   -> "https://trackiss.hateblo.jp",
      "Qiita"  -> "https://qiita.com/trackiss"
    )
) extends GitHubProfile
```
