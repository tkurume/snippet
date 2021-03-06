Morikatron Engineer Blog の記事 「[自動微分+XLA付き機械学習フレームワークJAXを使用してMNISTを学習させてみる](https://tech.morikatron.ai/entry/2020/12/07/100000)」のサンプルコードです。
詳しくはブログ記事を参照ください。

# 必要なライブラリのインストール手順
※Windowsには対応していません。Python 3.6以降。
```bash
pip install jax
pip install jaxlib
pip install scikit-learn
pip install tqdm
pip install tensorflow  # tf_sample.pyを動かす場合のみ
```
# ファイルリスト
* grad_sample.py
  * 簡単な関数を用いてJAXの自動微分機能を試すためのサンプルコード
* mlp_sample.py
  * 多層パーセプトロン(MLP)を用いてJAXの自動微分機能を試すためのサンプルコード
* mnist_sample.py
  * JAXによるMLPでMNISTデータセットを用いた分類タスクを学習させるためのサンプルコード
* mnist_sample_RMSProp.py
  * mnist_sample.pyのoptimizerをRMSPropに変更したコード
* tf_sample.py
  * mnist_sample.pyと同一のタスクをTensorflow2で行う場合のサンプルコード
