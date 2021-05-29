open node2vec.py and find :
args = ["C:\\Users\\Eagle3dStreaming\\Desktop\\GEM\\Snap-6.0-Win32\\node2vec.exe"]

update the path base don location of the folder so that it will point to the file:
......\GEM\Snap-6.0-Win32\node2vec.exe



than run in root folder:

python test_karate.py -node2vec 0 

python test_karate.py -node2vec 1


need to fix:
python test_sbm.py -node2vec 0
python test_sbm.py -node2vec 1
