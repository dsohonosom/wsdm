# idea
## 学習方法
- LoRAファインチューニング後、正しく予測できなかったデータを分析し新たな合成データを作成し学習
- LoRAファインチューニング後、正しく予測できなかったデータのみで学習（意味あるか？）
- Pseudo Labelingしたデータで学習後、trainデータで学習
- response_a/bで学習してresponse_b/aで予測、response_b/aで学習してresponse_a/bで予測
