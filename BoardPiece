import java.util.*;

public class BoardPiece {

	private KBNode[][] boardNodes;
	private boolean orientation;  // true = regular , false = botom up / 180 degree rotation 
	private Tile [][] tiles = new Tile[10][10];
 	
	public BoardPiece() {
        boardNodes = new KBNode[10][10];
        orientation = true;
    	}
	
	public BoardPiece(String boardString) {


        	for (int i = 0; i<boardString.length(); i++) {
           	int row = i/10;
            	int col = i%10;
            	boardNodes[row][col] = new KBNode();
            	boardNodes[row][col].setTerrainType(boardString.charAt(i));
        	}
    	}	

	
	public BoardPiece(String tileCodes) {
		int cnt = 0;
		for(int i = 0; i < 10; i++) {
			for (int j = 0; j < 10; j++) {
				tiles[i][j] = new Tile(tileCodes.charAt(cnt));
				cnt++;
			}
		}
	}
	
	public void setOrientation(Boolean b) {
        	orientation = b;
    	}
    
    	public KBNode[][] getBoard(){
    		return boardNodes;
    	}
	
}
