.PHONY: all clean

all: venv
	bash -c "source venv/bin/activate; RELEASE_MODE=1 jupyter nbconvert --to notebook --ExecutePreprocessor.timeout=3600 --execute Plots.ipynb"
	rm Plots.nbconvert.ipynb


venv:
	python3 -m venv venv
	bash -c "source venv/bin/activate; pip install -r requirements.txt"

clean:
	rm -f *.pdf
