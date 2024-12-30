# try & error

## モデル
- gemma-2-9b-itは速度面で学習・推論のいずれも遅い、精度はLlama-3.1-8B-Instructと差異なし
- Llama-3.1-8B-Instructは速度面で学習・推論のいずれも早い
- Qwen2.5-7B-Instructは速度面でLlama-3.1-8B-Instructと同程度で精度が高い
- Qwen2.5-14B-Instructは精度が高いが速度面で学習・推論のいずれも遅いのがネック→vLLMで予測できると推論時の速度向上が見込めるので試してみるか？

## 学習方法
- LoRAファインチューニング後、正しく予測できなかったデータを分析し新たな合成データを作成し学習
- LoRAファインチューニング後、正しく予測できなかったデータのみで学習（意味あるか？）
- Pseudo Labelingしたデータで学習後、trainデータで学習
- response_a/bで学習してresponse_b/aで予測、response_b/aで学習してresponse_a/bで予測→学習コストがかかるからやめとく？

# 推論方法
- 
