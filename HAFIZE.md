# Proje hedefi

Bu proje bir LLM ajanın kendi model ağırlıklarını (safetensors) güvenli bir sandbox'ta okuyup düzenleyebilmesi için gereken altyapıyı kodlar: 1) Tensor erişim katmanı (read/write), 2) Forward-pass sandbox (budgetlı inference), 3) Eval harness (MATH/GSM8K/IFEval), 4) Reviewer ajanı (bağımsız doğrulama), 5) İnsan onay kapısı (diff + regresyon raporu). Gerçek model ağırlıklarına erişim olmadığı için mock tensörlerle çalışır; API hazırlanır.
