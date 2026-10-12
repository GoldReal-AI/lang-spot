# lang-spot

Flags non-English words in mixed-language text.

**Model:** [goldreal-ai/lang-spot on Hugging Face](https://huggingface.co/goldreal-ai/lang-spot)

## Usage

```python
import sys
from huggingface_hub import snapshot_download

path = snapshot_download("goldreal-ai/lang-spot")
sys.path.insert(0, path)
from span_probes import load

probe = load(path)
probe.analyze("Vamos a la playa this weekend")
```

## License

CC BY-SA 4.0. See the model page for details.
